---
permalink: /
title: ""
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

# 大和 義英
所属： 東京大学 天文学専攻 相川研究室<br>東京大学大学院理学系研究科天文学専攻 修士課程2年<br>指導教員： [相川 祐理](https://www.astron.s.u-tokyo.ac.jp/members/doa/aikawa_yuri/)　教授

研究分野： 星・惑星形成、アストロケミストリー、原始惑星系円盤、電波天文学

ミリ波・サブミリ波の電波干渉計による高空間分解能観測を駆使して、星や惑星が形成される過程における物理進化・物質進化を明らかにすべく研究を行っています。

### プロジェクト
- Molecules with ALMA at Planet-forming Scales (MAPS) - The Chemistry of Planet Formation (ALMA Cycle 6 Large Program)
- Early Planet Formation in Embedded Disks (eDisk; ALMA Cycle 7 Large Program)
- Deuterium fractionation of ammonia in protostellar cores

## 近況

{% include base_path %}
{% assign recent_posts = site.posts | slice:0, 3 %}
{% for post in recent_posts %}
  {% if post.id %}
    {% assign title = post.title | markdownify | remove: "<p>" | remove: "</p>" %}
  {% else %}
    {% assign title = post.title %}
  {% endif %}
  <div class="list__item">
    <span style="font-size: 85%; color: grey; display:inline-block; width:8em;"><p class="page__date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | default: "1900-01-02" | date: "%Y.%m.%d" }}</time></p></span> <a href="{{ base_path }}{{ post.url }}" rel="permalink">{{ title }}</a>
  </div>
{% endfor %}

<p style="text-align:right" href="https://yyamato-as.github.io/website_jp/news/">More</p>

