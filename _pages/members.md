---
layout: page
title: members
permalink: /members/
# description: Members of MMAI Lab.
nav: true
nav_order: 7
display_categories: [PI, Students, Alumni]
horizontal: false
---

<!-- pages/members.md -->
<div class="members">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized members -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.members | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include members_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-4">
    {% for project in sorted_projects %}
      {% include members.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  <br>
  {% endfor %}

{% else %}

<!-- Display members without categories -->

{% assign sorted_projects = site.members | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include members_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-4">
    {% for project in sorted_projects %}
      {% include members.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
