---
layout: post
title: "Let'sえいごパズル! - 変化するキューブで楽しく学ぶ英単語"
permalink: /projects/2018/lets_eigo_puzzle
thumbnail: /assets/img/thumbnails/2018/lets_eigo_puzzle.png
description: "小学生が遊びながら英単語を学べる、赤外線通信ブロックとゲームを開発。"
---

{% assign pj = site.data.projects | where_exp: "pj", "pj.id == 'lets_eigo_puzzle'" | first %}

<img class='top-img lazyload' src='/assets/img/spinner.svg' alt='サムネイル画像' loading='lazy'
{% if pj.thumbnail == "tbu.png" %} data-src='https://img.youtube.com/vi/gqkjUVzhSBU/hqdefault.jpg'
{% else %}                         data-src='/assets/img/thumbnails/2018/lets_eigo_puzzle.png'
{% endif %}                        style='margin-bottom: 10px;' />

小学生が遊びながら英単語を学べる、赤外線通信ブロックとゲームを開発。

{% if pj.link %}
<a href="{{ pj.link }}" target="_blank" class="button">公式サイトを見る</a>
{% endif %}

### クリエータ
<p>
{% for creator_id in pj.creator_ids %}
  {% include creator.html is_simple=true %}
{% endfor %}
<small>(<a href='/projects/2018'>2018年度</a> 採択 / {% include link-to-mentor.html id=pj.mentor_id %}PM)</small>
</p>

{% if pj.comment %}
### PMコメント
<p class="project-comment">{{ pj.comment }}</p>
{% endif %}

## 発表動画
<div class="youtube">
  <iframe width="560" height="315" class="lazyload" data-src="https://www.youtube.com/embed/gqkjUVzhSBU?rel=0" frameborder="0" allowfullscreen=""></iframe>
</div>
<a href="https://www.youtube.com/watch?v={{ pj.youtube }}" target="_blank" rel="noopener" class="button">YouTube で見る</a>

{% include project-navigation.html %}

