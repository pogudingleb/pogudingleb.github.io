---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

## Preprints

{% for post in site.publications reversed %}
  {% if post.type == "preprint" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

## Peer-reviewed articles

{% for post in site.publications reversed %}
  {% if post.type == nil %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

## Other publications

{% for post in site.publications reversed %}
  {% if post.type == "other" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}


## Notes

{% for post in site.publications reversed %}
  {% if post.type == "note" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}


