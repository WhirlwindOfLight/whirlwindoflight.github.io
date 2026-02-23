---
title: Projects
nav_order: 1
---

## My Projects

<div class="project-grid">
  {% for project in site.data.projects %}
    {% include project_card.html %}
  {% endfor %}
</div>