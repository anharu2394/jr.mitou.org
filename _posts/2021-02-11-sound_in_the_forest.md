---
layout: post
title: "Sound in the forest - 複数のスマートフォンによる「動く音」の表現"
permalink: /projects/2018/sound_in_the_forest
thumbnail: /assets/img/thumbnails/2018/tbu.png
description: "複数のスマートフォン上のウェブブラウザをリアルタイム同期させ、立体音響を実現するシステムの開発。"
---

{% assign pj = site.data.projects | where_exp: "pj", "pj.id == 'sound_in_the_forest'" | first %}

<img class='top-img lazyload' src='/assets/img/spinner.svg' alt='サムネイル画像' loading='lazy'
{% if pj.thumbnail == "tbu.png" %} data-src='https://img.youtube.com/vi/H7SCFi0fp7g/hqdefault.jpg'
{% else %}                         data-src='/assets/img/thumbnails/2018/tbu.png'
{% endif %}                        style='margin-bottom: 10px;' />

複数のスマートフォン上のウェブブラウザをリアルタイム同期させ、立体音響を実現するシステムの開発。

### クリエータ（採択年度：<a href='/projects/2018'>2018年度</a>）
<p>
{% for creator_id in pj.creator_ids %}
  {% include creator.html is_simple=true %}
{% endfor %}
</p>

### メンター
<p>{% include link-to-mentor.html id=pj.mentor_id %}</p>

## 発表動画
<div class="youtube">
  <iframe width="560" height="315" class="lazyload" data-src="https://www.youtube.com/embed/H7SCFi0fp7g?rel=0" frameborder="0" allowfullscreen=""></iframe>
</div>
