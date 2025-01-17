---
layout: post
title: "fresh capsule - 食材管理アプリ"
permalink: /projects/2019/fresh_capsule
thumbnail: /assets/img/thumbnails/2019/fresh_capsule.jpg
description: "fresh capsuleは、購入した食材の賞味期限を管理する携帯アプリです。 賞味期限が印字されている部分をスマートフォンで撮影すると、賞味期限がアプリ内のリストに落とし込まれます。"
---

{% assign pj = site.data.projects | where_exp: "pj", "pj.id == 'fresh_capsule'" | first %}

<img class='top-img lazyload' src='/assets/img/spinner.svg' alt='サムネイル画像' loading='lazy'
{% if pj.thumbnail == "tbu.png" %} data-src='https://img.youtube.com/vi/vioFrqxlRXQ/hqdefault.jpg'
{% else %}                         data-src='/assets/img/thumbnails/2019/fresh_capsule.jpg'
{% endif %}                        style='margin-bottom: 10px;' />

fresh capsuleは、購入した食材の賞味期限を管理する携帯アプリです。 賞味期限が印字されている部分をスマートフォンで撮影すると、賞味期限がアプリ内のリストに落とし込まれます。

{% if pj.link %}
<a href="{{ pj.link }}" target="_blank" class="button">公式サイトを見る</a>
{% endif %}

### クリエータ
<p>
{% for creator_id in pj.creator_ids %}
  {% include creator.html is_simple=true %}
{% endfor %}
<small>(<a href='/projects/2019'>2019年度</a> 採択 / {% include link-to-mentor.html id=pj.mentor_id %}PM)</small>
</p>

{% if pj.comment %}
### PMコメント
<p class="project-comment">{{ pj.comment }}</p>
{% endif %}

## 発表動画
<div class="youtube">
  <iframe width="560" height="315" class="lazyload" data-src="https://www.youtube.com/embed/vioFrqxlRXQ?rel=0" frameborder="0" allowfullscreen=""></iframe>
</div>
<a href="https://www.youtube.com/watch?v={{ pj.youtube }}" target="_blank" rel="noopener" class="button">YouTube で見る</a>

{% include project-navigation.html %}

