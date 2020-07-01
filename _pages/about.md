---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I received my M.Sc. degree in Computer Science from the Federal University of Bahia (UFBA), in 2018, and my B.S. in Computer Networks from the Federal University of Ceará (UFC) in 2014.

More information, in my [Lattes curriculum](http://lattes.cnpq.br/3102385411862897){:target="_blank"} in Portuguese.

Latest five publications
------
<!--
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-pubs.html %}
  {% endfor %}</ul>
-->

<!-- I added this. Show only last-n-publications -->
  {% assign last-n-pub = 5 %}
  <ul>{% for post in site.publications reversed %}
    {% if forloop.index0 == last-n-pub %}
      {% break %}
    {% endif %}
    {% include archive-single-pubs.html %}
  {% endfor %}</ul>


<!-- Refs:
[1] https://shopify.github.io/liquid/tags/iteration/
[2] https://shopify.dev/docs/themes/liquid/reference/objects/for-loops
-->
