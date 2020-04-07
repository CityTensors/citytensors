---
title: "Sponsors"
layout: gridlay
excerpt: "Sponsors"
sitemap: false
permalink: /sponsors/
---

## NSF Awards ##

{% for sponsor in site.data.sponsors %}

  {{ sponsor.title }} <br />
  <em>{{ sponsor.authors }} </em>

  {% if sponsor.number_link == 1 %}
  <a href="{{ sponsor.link.url }}">{{ sponsor.link.display }}</a>
  {% endif %}

  {% if sponsor.number_link == 2 %}
  <a href="{{ sponsor.link1.url }}">{{ sponsor.link1.display }}</a>,
  <a href="{{ sponsor.link2.url }}">{{ sponsor.link2.display }}</a>
  {% endif %}

  {% if sponsor.number_link == 3 %}
  <a href="{{ sponsor.link1.url }}">{{ sponsor.link1.display }}</a>,
  <a href="{{ sponsor.link2.url }}">{{ sponsor.link2.display }}</a>,
  <a href="{{ sponsor.link3.url }}">{{ sponsor.link3.display }}</a>
  {% endif %}

  {% if sponsor.number_link == 4 %}
  <a href="{{ sponsor.link1.url }}">{{ sponsor.link1.display }}</a>,
  <a href="{{ sponsor.link2.url }}">{{ sponsor.link2.display }}</a>,
  <a href="{{ sponsor.link3.url }}">{{ sponsor.link3.display }}</a>,
  <a href="{{ sponsor.link4.url }}">{{ sponsor.link4.display }}</a>
  {% endif %}

{% endfor %}
