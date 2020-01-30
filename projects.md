---
layout: post
title: 未踏ジュニア採択プロジェクト
---

<div class="">
  <h2>採択プロジェクト</h2>
  <p>今までの採択プロジェクトです。☆はスーパークリエータに認定されました。</p>
  <a href="/projects/2019"><h3>2019年度</h3></a>
  <ul class="list-none">
    {% for pj in site.data.projects.nineteen %}
    <li>
      {% if pj.sp-creator %}
      <span>☆ </span>
      {% else %}
      <span>　 </span>
      {% endif %}
      {{pj.name}} {{pj.title}}
    </li>
    {% endfor %}
  </ul>
  <a href="/projects/2019" class="button">2019年度採択プロジェクト</a>
  <a href="/projects/2018"><h3>2018年度</h3></a>
  <ul class="list-none">
    {% for pj in site.data.projects.eighteen %}
    <li>
      {% if pj.sp-creator %}
      <span>☆ </span>
      {% else %}
      <span>　 </span>
      {% endif %}
      {{pj.name}} {{pj.title}}
    </li>
    {% endfor %}
  </ul>
  <a href="/projects/2018" class="button">2018年度採択プロジェクト</a>
  <a href="/projects/2017"><h3>2017年度</h3></a>
  <ul class="list-none">
    {% for pj in site.data.projects.seventeen %}
    <li>
      {% if pj.sp-creator %}
      <span>☆ </span>
      {% else %}
      <span>　 </span>
      {% endif %}
      {{pj.name}} {{pj.title}}
    </li>
    {% endfor %}
  </ul>
  <a href="/projects/2017" class="button">2017年度採択プロジェクト</a>
  <a href="/projects/2016"><h3>2016年度</h3></a>
  <ul class="list-none">
    {% for pj in site.data.projects.sixteen %}
    <li>
      {% if pj.sp-creator %}
      <span>☆ </span>
      {% else %}
      <span>　 </span>
      {% endif %}
      {{pj.name}} {{pj.title}}
    </li>
    {% endfor %}
  </ul>
  <a href="/projects/2016" class="button">2016年度採択プロジェクト</a>
</div>