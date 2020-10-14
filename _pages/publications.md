---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.
{% endif %}

{% include base_path %}

{% for year in (2019..2020) reversed %}
  <h2>{{ year }}</h2>
  {% for post in site.publications reversed %}
    {% if post.year == year %}
      {% include archive-single-publication.html%}
    {% endif %}
  {% endfor %}
{% endfor %}
