---
layout: academic
permalink: /
title: "Alessandro Giacardi"
description: "Development economist studying adaptation to shocks, risk perception, and food insecurity. PhD Candidate at Sapienza University of Rome."
author_profile: false
redirect_from:
  - /about/
  - /about.html
---
<style>
/* Homepage only: keep the portrait beside the introduction on desktop. */
.hero.home-hero {
  display: grid;
  grid-template-columns: minmax(0, 1fr) 250px;
  align-items: start;
  gap: 48px;
}
.home-hero .hero-copy {
  display: block;
  grid-column: 1;
  grid-row: 1;
  min-width: 0;
}
.home-hero .portrait {
  grid-column: 2;
  grid-row: 1;
  margin: 8px 0 0;
}
.home-hero .profiles {
  margin: 20px 0 0;
  gap: 8px 18px;
}
.home-hero .profiles a {
  min-height: 44px;
}
@media (max-width: 720px) {
  .hero.home-hero {
    grid-template-columns: minmax(0, 1fr);
    gap: 24px;
  }
  .home-hero .portrait {
    grid-column: 1;
    grid-row: 1;
    margin: 0;
  }
  .home-hero .portrait img {
    width: 120px;
    height: 148px;
  }
  .home-hero .hero-copy {
    grid-column: 1;
    grid-row: 2;
  }
  .home-hero h1 {
    margin: 0 0 22px;
  }
  .home-hero .hero-copy > p {
    margin: 0 0 18px;
  }
  .home-hero .actions {
    margin-top: 24px;
  }
}
</style>

<section class="hero home-hero" aria-labelledby="intro-title">
  <div class="hero-copy">
    <h1 id="intro-title">Alessandro Giacardi</h1>

    <p>I am a PhD Candidate in <a href="https://phd.uniroma1.it/web/SOCIAL-AND-ECONOMIC-SCIENCES_nD3759_EN.aspx">Development Economics</a> at Sapienza University of Rome and a Research Fellow at the <a href="https://www.cursa.it/project/progetto-osservatorio-sullinsicurezza-alimentare-nella-citta-metropolitana-di-roma-capitale-2022/">Food Insecurity and Poverty Observatory Lab</a>.</p>

    <p>I am an applied microeconomist working in development economics, with interests in adaptation strategies, agriculture, the environment, household decisions, and food security. I study how people and firms adapt to covariate shocks, with particular attention to risk perception, gender dynamics, and local risk management. My work spans Sub-Saharan Africa (Senegal and Uganda), Latin America (Mexico), Asia (China), and Italy.</p>

    <div class="actions">
      <a class="button primary" href="{{ '/research/' | relative_url }}">Explore research →</a>
      {% if site.cv_path != empty and site.cv_path %}
      <a class="cv-link" href="{{ site.cv_path | relative_url }}">CV <span class="filetype">PDF</span></a>
      {% endif %}
    </div>

    <div class="profiles" aria-label="Academic and professional profiles">
      {% for profile in site.data.profile_links %}
      <a href="{{ profile.url | escape }}">
        <span class="profile-icon {{ profile.icon }}" aria-hidden="true"></span>
        <span>{{ profile.label | escape }}</span>
      </a>
      {% endfor %}
    </div>
  </div>

  <figure class="portrait">
    <img src="{{ '/images/profile.jpg' | relative_url }}" alt="Alessandro Giacardi" width="250" height="300">
    <figcaption>Sapienza University of Rome · he/his</figcaption>
  </figure>
</section>

<section class="section" aria-label="Background">
  <p class="eyebrow">A little more about me</p>

  <p>In 2025/2026, I visited NOVA School of Business and Economics, hosted by NOVAFRICA. In 2024, I visited the Paris School of Economics within the Development Group. I have previously worked closely with national research communities (CREA) and several institutions and organizations (including the European Parliament, the Italian Parliament, UNESCO, and the Stockholm Environment Institute).</p>

  <p>Outside work, you can find me cooking, rowing, or tackling Arabic.</p>
</section>
