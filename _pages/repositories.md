---
layout: page
permalink: /repositories/
title: repositories
description: Edit the `_data/repositories.yml` and change the `github_users` and `github_repos` lists to include your own GitHub profile and repositories.
nav: true
nav_order: 4
---

<div class="alert alert-info" role="alert" markdown="1">
  <strong>Note:</strong> This page uses external services (github-readme-stats.vercel.app) to display repository cards. If cards are not loading or images appear broken, the external service may be experiencing downtime. 
  
  **Quick fixes:**
  - Visit your repositories directly on <a href="https://github.com/gcanasherrera" target="_blank">GitHub</a>
  - See [REPOSITORIES_TROUBLESHOOTING.md]({{ '/REPOSITORIES_TROUBLESHOOTING' | relative_url }}) for detailed solutions
  - **Best solution:** Deploy your own instance (free, ~10 minutes) following the <a href="https://github.com/anuraghazra/github-readme-stats#deploy-on-your-own" target="_blank">deployment guide</a>
</div>


{% if site.data.repositories.github_users %}

## GitHub users

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.liquid username=user %}
  {% endfor %}
</div>

---

{% if site.repo_trophies.enabled %}
{% for user in site.data.repositories.github_users %}
{% if site.data.repositories.github_users.size > 1 %}

  <h4>{{ user }}</h4>
  {% endif %}
  <div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% include repository/repo_trophies.liquid username=user %}
  </div>

---

{% endfor %}
{% endif %}
{% endif %}

{% if site.data.repositories.github_repos %}

## GitHub Repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
