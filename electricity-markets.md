---
layout: default
title: Electricity markets
permalink: /electricity-markets/
---

# Electricity markets

My opinions are my own.

---

## Posts

<ul class="post-list">
  {% assign posts = site.electricity_posts | sort: "date" | reverse %}
  {% for post in posts %}
    <li class="post-item">
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span class="muted"> — {{ post.date | date: "%Y-%m-%d" }}</span>
      {% if post.excerpt %}
        <div class="muted" style="margin-top:6px;">{{ post.excerpt | strip_html | truncate: 160 }}</div>
      {% endif %}
    </li>
  {% endfor %}
</ul>

<p class="muted" style="margin-top:18px;">
  To add a new post, create a file in <code>_electricity_posts/</code>.
</p>
