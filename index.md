---
title: オンライン ホステッド インストラクション
permalink: index.html
layout: home
ms.openlocfilehash: e096bbad394d45cb4fc4b50e3db13c1b5cc70433
ms.sourcegitcommit: 0398c15157de2f621dd945e76523b824e500901c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/23/2022
ms.locfileid: "145884056"
---
# <a name="content-directory"></a>コンテンツ ディレクトリ

各ケース スタディへのハイパーリンクを次に示します。

## <a name="case-studies"></a>ケース スタディ

{% assign casestudy = site.pages | where_exp:"page", "page.url contains '/Instructions/CaseStudy'" %}
| モジュール | ケース スタディ |
| --- | --- | 
{% for activity in casestudy  %}| {{ activity.casestudy.module }} | [{{ activity.casestudy.title }}{% if activity.casestudy.type %} - {{ activity.casestudy.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}
