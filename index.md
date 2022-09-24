---
title: オンラインでホスティングされている手順
permalink: index.html
layout: home
---

# <a name="content-directory"></a>コンテンツ ディレクトリ

各ケース スタディへのハイパーリンクを次に示します。

## <a name="case-studies"></a>ケース スタディ

{% assign casestudy = site.pages | where_exp:"page", "page.url contains '/Instructions/CaseStudy'" %}
| モジュール | ケース スタディ |
| --- | --- | 
{% for activity in casestudy  %}| {{ activity.casestudy.module }} | [{{ activity.casestudy.title }}{% if activity.casestudy.type %} - {{ activity.casestudy.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}
