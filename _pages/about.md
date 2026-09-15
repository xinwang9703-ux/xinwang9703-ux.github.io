---
layout: default
title: Home
permalink: /
nav: false
description: Xin Wang builds AI-enabled optimization and decision-support tools for supply chain planning.
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
      <a href="#contact">Contact</a>
    </nav>
  </aside>

  <div class="personal-content">
    <header class="personal-intro">
      <p class="personal-eyebrow">Operations research · AI · supply chain</p>
      <h2>Turning complex supply chain questions into decisions people can use.</h2>
      <p>I build AI-enabled optimization and decision-support solutions for supply chain planning. At Ashley Furniture, I work with cross-functional teams to frame operational questions, evaluate scenarios, and make cost, service, and network trade-offs easier to understand.</p>
    </header>

    <section aria-labelledby="focus-heading">
      <h2 id="focus-heading">What I work on</h2>
      <div class="personal-entry"><h3>Network design and decision-support agents</h3><p>Exploring network scenarios and translating optimization results into clear, business-facing choices.</p></div>
      <div class="personal-entry"><h3>Inventory optimization</h3><p>Balancing inventory investment, replenishment decisions, operating constraints, and service goals.</p></div>
      <div class="personal-entry"><h3>Ocean container loading</h3><p>Improving loading and utilization decisions while respecting practical capacity and operational constraints.</p></div>
      <a class="personal-text-link" href="{{ '/projects/' | relative_url }}">Explore selected work →</a>
    </section>

    <section aria-labelledby="approach-heading">
      <h2 id="approach-heading">How I work</h2>
      <p>I connect business context with technical delivery: identify the decision, understand the data and constraints, build an appropriate model or prototype, and communicate what the results mean. I care about solutions that are useful, transparent, scalable, and maintainable—not just technically interesting.</p>
      <p>My toolkit includes <strong>Python, SQL, Gurobi, optimization modeling, simulation, and data analysis</strong>.</p>
    </section>

    <section aria-labelledby="background-heading">
      <h2 id="background-heading">Background</h2>
      <p>I hold a Ph.D. from the National University of Singapore, an M.S. from the University of North Carolina at Chapel Hill, and a B.S. from Shanghai Jiao Tong University. My research training in operations research and statistics supports the practical decision systems I build today.</p>
    </section>

    <section id="contact" aria-labelledby="contact-heading">
      <h2 id="contact-heading">Get in touch</h2>
      <p>I enjoy connecting with people working on supply chain analytics, optimization, and AI-enabled decision support. The best way to reach me is by email; you can also find my work on <a href="https://github.com/{{ site.data.socials.github_username }}" target="_blank" rel="noopener noreferrer">GitHub</a>.</p>
      <div class="personal-contact-links">{% social_links %}</div>
    </section>

  </div>
</div>
