---
title: オンライン ホステッド インストラクション
permalink: index.html
layout: home
---

# コンテンツ ディレクトリ

各ケース スタディへのハイパーリンクを以下に一覧表示します。

## ケース スタディ

{% assign casestudy = site.pages | where_exp:"page", "page.url contains '/Instructions/CaseStudy'" %}
| モジュール | ケース スタディ |
| --- | --- | 
{% for activity in casestudy  %}| {{ activity.casestudy.module }} | [{{ activity.casestudy.title }}{% if activity.casestudy.type %} - {{ activity.casestudy.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}
