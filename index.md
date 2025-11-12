---
layout: default
title: InnerVault Journal
---

# InnerVault Journal

Welcome to **InnerVault** — a growing vault of documented systems, insights, and experiments.  
Use the filters below to explore specific topics.

---

## 🧠 Filter by Category

<div id="filter-bar">
  <button class="filter-btn active" data-filter="all">All</button>
  {% assign categories = site.posts | map: 'categories' | join: ',' | split: ',' | uniq %}
  {% for category in categories %}
    {% unless category == "" %}
      <button class="filter-btn" data-filter="{{ category | strip }}">{{ category | capitalize }}</button>
    {% endunless %}
  {% endfor %}
</div>

<div class="post-grid">

{% for post in site.posts %}
  <article class="post-card fade-in" data-category="{{ post.categories | join: ' ' }}">
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

*“Each category reveals a different layer of the vault.”*

<script>
  // ✦ InnerVault Category Filter ✦
  const buttons = document.querySelectorAll('.filter-btn');
  const posts = document.querySelectorAll('.post-card');

  buttons.forEach(btn => {
    btn.addEventListener('click', () => {
      // Remove active state
      buttons.forEach(b => b.classList.remove('active'));
      btn.classList.add('active');

      const filter = btn.dataset.filter;

      posts.forEach(post => {
        const category = post.dataset.category;
        if (filter === 'all' || category.includes(filter)) {
          post.style.display = 'block';
        } else {
          post.style.display = 'none';
        }
      });
    });
  });
</script>
