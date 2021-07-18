# Inicio
Wikipedia del TEA
<div class="git-wiki-page-list">
    ## Paginas:
    <ul class="page-list">
        {% assign items = site.html_pages | sort: 'date' %} {% for page in items %}
        {% if page.is_wiki_page != false and page.sitemap != false %}
        <li class="page-list-item">
            {% assign title = page.title | default: page.name %}
            <a href="{{ page.url | relative_url }}">{{title | escape}}</a>
        </li>
{% endif %}
        {% endfor %}
    </ul>
</div>
