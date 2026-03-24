---
title: People
permalink: /people/
classes: wide
---

## Faculty

<div class="grid__wrapper">
{% assign faculty = site.people | where: "type", "faculty" | sort: "last_name" %}
{% for person in faculty %}
  {% include person-grid.html %}
{% endfor %}
</div>

<div style="clear: both;"></div>

## Research Fellows and Postdocs

<div class="grid__wrapper">
{% assign postdocs = site.people | where: "type", "postdoc" | sort: "last_name" %}
{% for person in postdocs %}
  {% include person-grid.html %}
{% endfor %}
</div>

<div style="clear: both;"></div>

## Research support staff

<div class="grid__wrapper">
{% assign support_staff = site.people | where: "type", "support" | sort: "last_name" %}
{% for person in support_staff %}
  {% include person-grid.html %}
{% endfor %}
</div>

<div style="clear: both;"></div>

## PhD Students

<div class="grid__wrapper">
{% assign phd_students = site.people | where: "type", "phd" | sort: "last_name" %}
{% for person in phd_students %}
  {% include person-grid.html %}
{% endfor %}
</div>

<div style="clear: both;"></div>

## Masters-by-Research Students

<div class="grid__wrapper">
{% assign mscr_students = site.people | where: "type", "mscr" | sort: "last_name" %}
{% for person in mscr_students %}
  {% include person-grid.html %}
{% endfor %}
</div>

<div style="clear: both;"></div>
