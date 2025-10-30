---
layout: single
title: "Publications"
author_profile: true
permalink: /publications/
classes: wide
---
{% assign pubyears = site.publications | group_by:"year"  %}
{% assign sorted_pubyears = pubyears | reverse %}
{% for year in sorted_pubyears %}
## {{ year.name }}
{:#y{{ year.name }} .year}
{% for pub in year.items %}
  {% include publication.html pub=pub %}
{% endfor %}
{% endfor %}