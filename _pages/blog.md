---
layout: default
permalink: /blog/
title: Writing
nav: true
nav_order: 3
description: Notes on operations research, supply chain analytics, and applied AI.
---

<link rel="stylesheet" href="{{ '/assets/css/personal-site.css' | relative_url }}">

<div class="personal-layout">
  <aside class="personal-profile" aria-label="Profile">
    <div class="personal-monogram" aria-hidden="true">XW</div>
    <h1>Xin Wang</h1>
    <p>AI Research Scientist<br>Supply Chain Optimization</p>
    <nav class="personal-profile-links" aria-label="Profile links">
      <a href="{{ '/cv/' | relative_url }}">CV</a>
      <a href="https://github.com/{{ site.data.socials.github_username }}" target="_blank" rel="noopener noreferrer">GitHub</a>
      <a href="{{ '/' | relative_url }}#contact">Contact</a>
    </nav>
  </aside>

  <div class="personal-content">
    <header class="personal-intro">
      <p class="personal-eyebrow">Ideas and practical notes</p>
      <h2>Writing</h2>
      <p>Notes on optimization modeling, supply chain analytics, simulation, and how to turn analysis into usable decision support. I share reusable methods and lessons, not confidential company details.</p>
    </header>

    {% for post in site.posts %}
      <article class="personal-entry personal-writing-entry">
        <p class="personal-entry-date">{{ post.date | date: '%B %Y' }}</p>
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        {% if post.description %}<p>{{ post.description }}</p>{% endif %}
      </article>
    {% endfor %}

    {% if site.posts.size == 0 %}<p>New notes will appear here soon.</p>{% endif %}

  </div>
</div>
