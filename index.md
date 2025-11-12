---
layout: default
title: InnerVault Journal
---

# InnerVault Journal

Welcome to **InnerVault** — my personal vault of thoughts, systems, and documented evolution.  
Each post here is a fragment of process — a snapshot of learning, building, and refining.

---

## 🧩 The Vault Feed

<div class="post-grid">

{% for post in site.posts %}
  <article class="post-card fade-in">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
    <p class="excerpt">
      {{ post.excerpt | strip_html | truncate: 140 }}
    </p>
    <a href="{{ post.url }}" class="read-more">→ Read more</a>
  </article>
{% endfor %}

</div>

---

*“Every post is a vault key — a log in the evolution of thought.”*
