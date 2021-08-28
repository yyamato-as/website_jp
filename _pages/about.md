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

## 最近のニュース

{% include base_path %}
{% for post in site.posts %}
  {% if post.id %}
    {% assign title = post.title | markdownify | remove: "<p>" | remove: "</p>" %}
  {% else %}
    {% assign title = post.title %}
  {% endif %}
  <div class="list__item">
    {% if post.link %}
      <a href="{{ post.link }}">{{ title }}</a> <a href="{{ base_path }}{{ post.url }}" rel="permalink"><i class="fa fa-link" aria-hidden="true" title="permalink"></i><span class="sr-only">Permalink</span></a>
    {% else %}
      <a href="{{ base_path }}{{ post.url }}" rel="permalink">{{ title }}</a>
    {% endif %}
  </div>
{% endfor %}


- 2021.8.13 ALMA Cycle 8 2021 の観測プロポーザルがグレードBで採択されました。

