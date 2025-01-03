---
title: "remino@github"
---

# {{ site.title }}

**👋 Hi, I'm Rem, a Web developer in Japan.**  
Above is a link to my profile, and below are my public repos of scripts and other things on GitHub.

---

{% for repo in site.data.repos %}
[{{ repo.name }}]({% if repo.homepageUrl != "" %}{{ repo.homepageUrl }}{% else %}{{ repo.url }}{% endif %})
: {{#repo.description}}{{ repo.description }}.{{/repo.description}}{{^repo.description}}Repository.{{/repo.description}}

{% endfor %}

[github]: https://github.com/remino
