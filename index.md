---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
# .public_repositories

layout: home
---

{% for page in site.pages %}
    <url>
        <loc>http://blog.dside.ru{{ page.url | remove: 'index.html' }}</loc>
    </url>
    {% endfor %}

{% for repo in site.github limit:5 %} <a href = "{{repo.html_url}}">{{repo.name}}</a><br> {%endfor%}
