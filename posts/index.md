---
layout: layout.njk
title: ブログ一覧
---
# {{ title }}

## ページ一覧（Collections）

{% for post in collections.post %}
  - [{{ post.data.title }}](/posts/{{ post.fileSlug }})
{% endfor %}

## ユーザ一覧（Golobal Data Files）

{% for user in userList %}
  - {{ user }}
{% endfor %}
