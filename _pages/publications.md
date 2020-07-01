---
<!--layout: archive-->
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

{% if page.author and site.data.authors[page.author] %}
  {% assign author = site.data.authors[page.author] %}
{% else %}
  {% assign author = site.author %}
{% endif %}

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{ author.googlescholar }}" target="_blank">my Google Scholar profile</a>.</u>
{% endif %}

<!-- I comment this. Origin code.
{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %} -->

<!-- New code. Link bellow to categories (category-archive.html) page -->
> Show publications in [more detail]({{ base_path }}/categories).

<!-- I copy this block code from the _pages/category-archive.html file, to show publications sorted by category -->
{% include group-by-array collection=site.publications field="categories" %}

{% for category in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ category | slugify }}" class="archive__subtitle">{{ category | capitalize }}</h2>
  <ol reversed>{% for post in posts reversed %}
    {% include archive-single-pubs.html %}
  {% endfor %}</ol>
{% endfor %}
