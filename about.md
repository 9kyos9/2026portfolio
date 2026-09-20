---
layout: default
title: About
permalink: /about/
---

<h1>About</h1>

<p class="lead">
  I'm {{ site.author }}, an AI Engineer focused on building LLM-powered
  products and machine learning systems that ship. Rewrite this with your
  own story, interests, and what kind of role you're looking for.
</p>

<h2>Experience</h2>
<div class="timeline">
  {% for job in site.data.experience.work %}
    <div class="timeline-item">
      <div class="timeline-head">
        <strong>{{ job.role }}</strong>
        <span class="muted">{{ job.org }} · {{ job.period }}</span>
      </div>
      <ul>
        {% for p in job.points %}<li>{{ p }}</li>{% endfor %}
      </ul>
    </div>
  {% endfor %}
</div>

<h2>Education</h2>
<div class="timeline">
  {% for ed in site.data.experience.education %}
    <div class="timeline-item">
      <div class="timeline-head">
        <strong>{{ ed.degree }}</strong>
        <span class="muted">{{ ed.org }} · {{ ed.period }}</span>
      </div>
      <ul>
        {% for p in ed.points %}<li>{{ p }}</li>{% endfor %}
      </ul>
    </div>
  {% endfor %}
</div>

<h2>Get in touch</h2>
<ul>
  <li>Email: <a href="mailto:{{ site.email }}">{{ site.email }}</a></li>
  <li>GitHub: <a href="https://github.com/{{ site.github_username }}">@{{ site.github_username }}</a></li>
</ul>
