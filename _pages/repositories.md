---
layout: page
permalink: /repositories/
title: repositories
description:
nav: true
nav_order: 4
---

A selection of model implementations, toolboxes and general software developed by our group. For a full overview, visit our [GitHub organization](https://github.com/bioAI-Oslo).

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
