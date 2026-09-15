---
layout: default
title: Work
permalink: /projects/
description: Selected industry and research work in optimization, analytics, and decision support.
nav: true
nav_order: 2
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
      <p class="personal-eyebrow">Selected work</p>
      <h2>Industry projects</h2>
      <p>These are public-safe summaries of the problems and methods I work with. Project-specific implementation details and results will be added only after review for public sharing.</p>
    </header>

    {% assign industry_projects = site.projects | where: "category", "industry" | sort: "importance" %}
    {% for project in industry_projects %}
      <article class="personal-entry">
        <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
        <p>{{ project.description }}</p>
      </article>
    {% endfor %}

    <section aria-labelledby="research-heading">
      <h2 id="research-heading">Research foundations</h2>
      <p>My research background helps me handle uncertainty, constraints, and complex systems in practical decision-making.</p>
      {% assign research_projects = site.projects | where: "category", "research" | sort: "importance" %}
      {% for project in research_projects %}
        <article class="personal-entry">
          <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
          <p>{{ project.description }}</p>
        </article>
      {% endfor %}
    </section>

  </div>
</div>
