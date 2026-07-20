---
layout: default
title: "AI시민연구소 블로그"
---

<section class="hero">
  <p class="eyebrow">AI Citizen Lab · Public AI Literacy</p>
  <h1>AI를 어렵지 않게, 사람에게 이롭게.</h1>
  <p>AI시민연구소는 매일 쏟아지는 AI 뉴스 중 시민에게 실제로 도움이 되는 주제 하나를 골라 쉽고 재미있게 해석합니다.</p>
  <div class="cta-row">
    <a class="button" href="{{ '/about/' | relative_url }}">연구소 소개</a>
    <a class="button ghost" href="#latest">최신 글 보기</a>
  </div>
</section>

<section class="principles">
  <div><strong>공익성</strong><span>AI 정보 격차를 줄입니다.</span></div>
  <div><strong>쉬운 해설</strong><span>전문용어를 생활 언어로 바꿉니다.</span></div>
  <div><strong>검증</strong><span>공식 출처와 날짜를 확인합니다.</span></div>
  <div><strong>인간 중심</strong><span>AI보다 사람이 먼저입니다.</span></div>
</section>

<section id="latest">
  <h2>최신 포스팅</h2>
  <div class="post-list">
    {% for post in site.posts limit:12 %}
      <article class="post-card">
        {% if post.image %}
        <a class="post-thumb-link" href="{{ post.url | relative_url }}" aria-label="{{ post.title }}">
          <img src="{{ post.image | relative_url }}" alt="{{ post.image_alt | default: post.title }}" loading="lazy">
        </a>
        {% endif %}
        <p class="date">{{ post.date | date: "%Y.%m.%d" }}</p>
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <p>{{ post.description | default: post.excerpt | strip_html | truncate: 140 }}</p>
        <a class="read-more" href="{{ post.url | relative_url }}">읽기 →</a>
      </article>
    {% endfor %}
  </div>
</section>
