---
layout: post
title: "VRSandbox：誰でも簡単3Dモデリングツール"
permalink: /projects/2021/vr_sandbox
thumbnail: /assets/img/thumbnails/2021/vr_sandbox.png
description: "VRコントローラーを筆とパレットのように使い、直感的に立体物が作れるアプリです。仮想空間や３Dモデルが身近になりましたが、現状で個人が作るのは簡単ではありません。難解なモデリングソフトを使用しなくても簡単に３Dモデリングできます。しゃがむアクションで縮尺が変わり、実物大の建造物に入れます。"
---

{% assign pj = site.data.projects | where_exp: "pj", "pj.id == 'vr_sandbox'" | first %}

<img class='top-img lazyload' src='/assets/img/spinner.svg' alt='サムネイル画像' loading='lazy'
{% if pj.thumbnail == "tbu.png" %} data-src='/assets/img/thumbnails/tbu.png'
{% else %}                         data-src='/assets/img/thumbnails/{{ pj.year }}/{{ pj.thumbnail }}'
{% endif %}                        style='margin-bottom: 10px; border-radius: 6px;' />

{{ pj.description }}

<div style='display: flex; flex-wrap: wrap'>
  {% if pj.link %}
  <a href="{{ pj.link }}" target="_blank" class="button">公式サイトを見る</a>
  {% endif %}

  <a href="https://twitter.com/intent/tweet?text={{ pj.title }}&via=MitouJr&hashtags=未踏ジュニア&related=MitouJr&lang=jp&url={{ site.url }}/projects/{{ pj.year }}/{{ pj.id }}" class="button" target="_blank" rel="noopener">ツイートする</a>
</div>

### クリエータ
<p>
  {% for creator_id in pj.creator_ids %}
    {% include creator.html is_simple=true %}
  {% endfor %}
  <small>(<a href='/projects/{{ pj.year }}'>{{ pj.year }}年度</a> 採択 / {% include link-to-mentor.html id=pj.mentor_id %}PM)</small>
</p>

{% if pj.comment %}
### PMコメント
<p class="project-comment">{{ pj.comment }}</p>
{% endif %}

{% if pj.youtube != 'TBD' %}
## 紹介動画
<div class="youtube">
  <iframe width="560" height="315" class="lazyload" data-src="https://www.youtube.com/embed/{{ pj.youtube }}?rel=0" frameborder="0" allowfullscreen=""></iframe>
</div>
<a href="https://www.youtube.com/watch?v={{ pj.youtube }}" target="_blank" rel="noopener" class="button">YouTube で見る</a>
{% endif }

{% include project-navigation.html %}
