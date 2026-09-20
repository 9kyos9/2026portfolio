---
layout: default
title: 소개
permalink: /about/
---

<h1>소개</h1>

<p class="lead">
  안녕하세요, 데이터와 AI 모델링을 통해 실질적인 가치를 도출하는 길을 탐구하는
  김은교입니다. 그래프 기반 딥러닝, LLM·RAG 애플리케이션, 데이터 분석 프로젝트를
  수행해 왔습니다.
</p>

<h2>학력</h2>
<div class="timeline">
  {% for ed in site.data.experience.education %}
    <div class="timeline-item">
      <div class="timeline-head">
        <strong>{{ ed.org }}</strong>
        <span class="muted">{{ ed.period }}</span>
      </div>
      <p class="muted" style="margin:4px 0 0">{{ ed.degree }}</p>
    </div>
  {% endfor %}
</div>

<h2>대내외 활동</h2>
<div class="timeline">
  {% for a in site.data.experience.activities %}
    <div class="timeline-item">
      <div class="timeline-head">
        <strong>{{ a.name }}</strong>
        <span class="muted">{{ a.period }}</span>
      </div>
      <p class="muted" style="margin:4px 0 0">{{ a.detail }}</p>
    </div>
  {% endfor %}
</div>

<h2>수상 내역</h2>
<div class="timeline">
  {% for w in site.data.experience.awards %}
    <div class="timeline-item">
      <div class="timeline-head">
        <strong>{{ w.name }}</strong>
        <span class="muted">{{ w.date }}</span>
      </div>
      {% if w.detail %}<p class="muted" style="margin:4px 0 0">{{ w.detail }}</p>{% endif %}
    </div>
  {% endfor %}
</div>

<h2>어학 및 자격증</h2>
<div class="timeline">
  {% for c in site.data.experience.certifications %}
    <div class="timeline-item">
      <div class="timeline-head">
        <strong>{{ c.name }}</strong>
        <span class="muted">{{ c.date }}</span>
      </div>
    </div>
  {% endfor %}
</div>

<h2>연락처</h2>
<ul>
  <li>이메일: <a href="mailto:{{ site.email }}">{{ site.email }}</a></li>
  <li>GitHub: <a href="https://github.com/{{ site.github_username }}">@{{ site.github_username }}</a></li>
  {% if site.linkedin_username and site.linkedin_username != "" %}<li>LinkedIn: <a href="https://www.linkedin.com/in/{{ site.linkedin_username }}">{{ site.linkedin_username }}</a></li>{% endif %}
</ul>
