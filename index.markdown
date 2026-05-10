---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Miika Kanerva
---

<section class="project-section" aria-labelledby="featured-projects">
  <h2 id="featured-projects">About</h2>

  <p>
    Unity developer based in Espoo, Finland. I've been programming and working on games since 2015, and am one of the co-founders of Improx Games founded in 2016. I'm also one of the owners of an indie studio Mopeful Games since 2021.
  </p>
</section>

<section class="project-section" aria-labelledby="featured-projects">
  <h2 id="featured-projects">Featured Work</h2>

  <div class="featured-stack">
    {% for project in site.data.games.featured %}
      {% include featured-project.html project=project %}
    {% endfor %}
  </div>
</section>

<section class="project-section" aria-labelledby="other-projects">
  <h2 id="other-projects">Projects</h2>

  <div class="jam-grid">
    {% for project in site.data.games.projects %}
      {% include jam-card.html project=project %}
    {% endfor %}
  </div>
</section>

<section class="project-section" aria-labelledby="smaller-projects">
  <h2 id="smaller-projects">Game Jams & Smaller Projects</h2>

  <div class="jam-grid">
    {% for project in site.data.games.jams %}
      {% include jam-card.html project=project %}
    {% endfor %}
  </div>
</section>
