---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Miika Kanerva
---

<section class="project-section" aria-labelledby="about">
  <h2 id="about">About</h2>

  <p>
    Unity developer based in Espoo, Finland, focused on gameplay systems,
    technical implementation, and shipping games across PC and consoles. I have
    been making games since 2015, co-founded Improx Games in 2016, and have
    been one of the owners of indie studio Mopeful Games since 2021.
  </p>

  <p>
    Contact: maikkanerva@gmail.com
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
