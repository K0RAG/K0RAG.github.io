---
layout: default
title: My Work
---

# My Work

This page lists my repositories, folders, and files.

---
## 🔗 GitHub Repositories (Auto-fetched)

{% if site.github.public_repositories %}
{% for repo in site.github.public_repositories %}
{% unless repo.name == "K0RAG.github.io" %}

### 🔹 [{{ repo.name }}]({{ repo.html_url }})

{{ repo.description }}

⭐ Stars: {{ repo.stargazers_count }}

---
{% endunless %}
{% endfor %}
{% else %}
GitHub repositories could not be loaded.
{% endif %}

## 📁 Project Structure Example

```text
AI-Project/
├── data/
│   └── dataset.csv
├── models/
│   └── svm.py
├── notebooks/
│   └── analysis.ipynb
└── README.md
