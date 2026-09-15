---
layout: default
title: Beyond Work
permalink: /beyond-work/
description: A selective glimpse of the person behind the work.
nav: true
nav_order: 4
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
      <p class="personal-eyebrow">The person behind the work</p>
      <h2>Beyond work</h2>
      <p>A small, intentionally selective glimpse of what gives me energy and perspective outside the office.</p>
    </header>

    <section aria-labelledby="personality-heading">
      <h2 id="personality-heading">Personality</h2>
      <p>I am an <strong>{{ site.data.personal.mbti.type }}</strong>—people-oriented, practical, and usually happiest when the people around me feel supported. I take the four letters lightly, but that part sounds about right.</p>
    </section>

    <section aria-labelledby="family-heading">
      <h2 id="family-heading">Family</h2>
      <p>My husband and our son are at the heart of my life outside work. I love them deeply, and they give me strength, perspective, and the kind of everyday wisdom that no textbook can teach.</p>
    </section>

    <section aria-labelledby="interests-heading">
      <h2 id="interests-heading">Things I enjoy</h2>
      <div class="personal-entry"><h3>Ultimate frisbee</h3><p>The pace, teamwork, and shared energy of the game.</p></div>
      <div class="personal-entry"><h3>Violin</h3><p>A quieter, more focused creative space.</p></div>
      <div class="personal-entry"><h3>Nail art</h3><p>Experimenting with color, detail, and small-scale design.</p></div>
      <div class="personal-entry"><h3>Swimming</h3><p>A way to reset, stay active, and clear my mind.</p></div>
    </section>

    <section aria-labelledby="photos-heading">
      <h2 id="photos-heading">Photo journal</h2>
      {% assign life_photos = site.data.life_photos.photos %}
      {% if life_photos and life_photos.size > 0 %}
        <div class="personal-photo-grid">
          {% for photo in life_photos %}
            <figure>
              <img src="{{ photo.path | relative_url }}" alt="{{ photo.alt | escape }}" loading="lazy">
              {% if photo.caption %}<figcaption>{{ photo.caption }}</figcaption>{% endif %}
            </figure>
          {% endfor %}
        </div>
      {% else %}
        <p>A few carefully chosen moments will appear here soon.</p>
      {% endif %}
    </section>

  </div>
</div>
