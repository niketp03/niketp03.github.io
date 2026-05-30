---
layout: page
permalink: /repositories/
title: repositories
description:
nav: true
nav_order: 3
---

{% if site.data.repositories.github_repos %}
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
{% endif %}
