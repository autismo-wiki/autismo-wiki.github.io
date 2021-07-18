# Inicio
Wikipedia del TEA
<div class="git-wiki-page-list">
    <span class="page-list-title">Paginas:</span>
    <ul class="page-list">
        {% assign items = site.html_pages %} {% for page in items %}
        <li class="page-list-item">
            {% assign title = page.title | default: page.name %}
            <a href="{{ page.url | relative_url }}">{{title | escape}}</a>
        </li>
        {% endfor %}
    </ul>
</div>
