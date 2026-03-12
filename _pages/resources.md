---
title: Resources
permalink: /resources/
classes: wide
---

A collection of datasets, software, and resources developed by BGC members.

## Software

<div class="grid__wrapper">
{% assign software = site.resources | where: "type", "software" | sort: "title" %}
{% for resource in software %}
  {% include resource-grid.html %}
{% endfor %}
</div>

<div style="clear: both;"></div>

## Hardware

<div class="grid__wrapper">
{% assign hardware = site.resources | where: "type", "hardware" | sort: "title" %}
{% for resource in hardware %}
  {% include resource-grid.html %}
{% endfor %}
</div>

<div style="clear: both;"></div>

## Facilities

<div class="grid__wrapper">
{% assign facilities = site.resources | where: "type", "facilities" | sort: "title" %}
{% for resource in facilities %}
  {% include resource-grid.html %}
{% endfor %}
</div>

<div style="clear: both;"></div>

## Datasets

<div class="grid__wrapper">
{% assign datasets = site.resources | where: "type", "datasets" | sort: "title" %}
{% for resource in datasets %}
  {% include resource-grid.html %}
{% endfor %}
</div>

<div style="clear: both;"></div>

## Group Resources

<div class="grid__wrapper">
{% assign group = site.resources | where: "type", "group" | sort: "title" %}
{% for resource in group %}
  {% include resource-grid.html %}
{% endfor %}
</div>

<div style="clear: both;"></div>
