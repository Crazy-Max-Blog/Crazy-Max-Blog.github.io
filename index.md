---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
# 

layout: home
---
<meta name="yandex-verification" content="c1d96685742fc61d" />

{% for page in site.pages %}
    <url>
        <loc>http://blog.dside.ru{{ page.url | remove: 'index.html' }}</loc>
    </url>
    {% endfor %}

{% for repo in site.github.public_repositories limit:5 %} <a href = "/{{repo.name}}">{{repo.name}}</a><br> {%endfor%}
