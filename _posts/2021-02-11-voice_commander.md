---
layout: post
title: "Voice Commander ～命令×ポーズ×チェス～"
permalink: /projects/2016/voice_commander
thumbnail: /assets/img/thumbnails/2016/tbu.png
description: "Voice Commanderは、声とジェスチャーで操作する新感覚チェスゲームです。 グラフィックにこだわるだけでなく、音声認識によるコマの操作、スマホに表示したマーカーを利用したジェスチャー操作等を組み合わせることで、「かっこよさ」を追求しています。 アニメ「ノーゲーム・ノーライフ」に出てきたチェスから着想を得て開発をすすめました。 それぞれのマスにはプレーヤーが音声認識の際に叫ぶための名前がついていて、テキストファイルを変更することで簡単に名前をカスタマイズすることもできます。"
---

{% assign pj = site.data.projects | where_exp: "pj", "pj.id == 'voice_commander'" | first %}

<img class='top-img lazyload' src='/assets/img/spinner.svg' alt='サムネイル画像' loading='lazy'
{% if pj.thumbnail == "tbu.png" %} data-src='https://img.youtube.com/vi/APUTGg6g0hA/hqdefault.jpg'
{% else %}                         data-src='/assets/img/thumbnails/2016/tbu.png'
{% endif %}                        style='margin-bottom: 10px;' />

Voice Commanderは、声とジェスチャーで操作する新感覚チェスゲームです。 グラフィックにこだわるだけでなく、音声認識によるコマの操作、スマホに表示したマーカーを利用したジェスチャー操作等を組み合わせることで、「かっこよさ」を追求しています。 アニメ「ノーゲーム・ノーライフ」に出てきたチェスから着想を得て開発をすすめました。 それぞれのマスにはプレーヤーが音声認識の際に叫ぶための名前がついていて、テキストファイルを変更することで簡単に名前をカスタマイズすることもできます。

{% if pj.link %}
<a href="{{ pj.link }}" target="_blank" class="button">公式サイトを見る</a>
{% endif %}

### クリエータ
<p>
{% for creator_id in pj.creator_ids %}
  {% include creator.html is_simple=true %}
{% endfor %}
<small>(<a href='/projects/2016'>2016年度</a> 採択 / {% include link-to-mentor.html id=pj.mentor_id %}PM)</small>
</p>

{% if pj.comment %}
### PMコメント
<p class="project-comment">{{ pj.comment }}</p>
{% endif %}

## 発表動画
<div class="youtube">
  <iframe width="560" height="315" class="lazyload" data-src="https://www.youtube.com/embed/APUTGg6g0hA?rel=0" frameborder="0" allowfullscreen=""></iframe>
</div>
<a href="https://www.youtube.com/watch?v={{ pj.youtube }}" target="_blank" rel="noopener" class="button">YouTube で見る</a>

{% include project-navigation.html %}

