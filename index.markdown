---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Miika Kanerva
---

<section class="games-intro">
  <p>
    Game developer portfolio featuring larger production work, technical
    contributions, and smaller game jam projects.
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

<section class="project-section" aria-labelledby="smaller-projects">
  <h2 id="smaller-projects">Game Jams & Smaller Projects</h2>

  <div class="jam-grid">
    {% for project in site.data.games.jams %}
      {% include jam-card.html project=project %}
    {% endfor %}
  </div>
</section>
