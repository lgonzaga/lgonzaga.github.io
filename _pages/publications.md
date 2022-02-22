---
layout: archive
title: "Publications (last papers)"
permalink: /publications/
author_profile: true
---
For a complete list of papers, access: <https://www.researchgate.net/profile/Luiz-Gonzaga-Da-Silveira-Jr>   

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
