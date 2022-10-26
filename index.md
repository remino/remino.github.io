---
title: "remino@github"
---
# ![remino logo][logo] {{ site.title }}

[github.com/remino][github]
: **👋 Hi, I'm Rem, a Web developer in Japan.**  
Above is a link to my profile, and below are my public repos of scripts and other things on GitHub.

---

{% for repo in site.data.repos %}
[{{ repo.name }}]({% if repo.homepageUrl != "" %}{{ repo.homepageUrl }}{% else %}{{ repo.url }}{% endif %})
: {{ repo.description }}.

{% endfor %}

[github]: https://github.com/remino
[logo]: https://avatars.githubusercontent.com/u/29999
