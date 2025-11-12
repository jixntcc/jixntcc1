---
layout: page
title: Archive
permalink: /archive/
---

# 🗂 Archive

A complete record of everything published in **InnerVault Journal** — thoughts, lessons, and experiments collected over time.  
Each post here marks a version of growth — a captured idea in the ongoing process of refinement.

---

## 🕰 All Entries

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }})  
  *{{ post.date | date: "%B %d, %Y" }}* — {{ post.categories | join: ", " }}
{% endfor %}

---

## 💭 About This Archive

This list is intentionally linear — no filters, no complexity.  
Just time, effort, and the path of ideas as they evolved.  

Every post is part of the system: **observe → document → refine → evolve**.

---

*“Everything recorded here is a timestamp in thought — a log of becoming.”*
