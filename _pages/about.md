---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a Ph.D. student in Computer Science at the [Federal University of Bahia](http://pgcomp.dcc.ufba.br){:target="\_blank"}. I am advised by [Prof. Leobino Sampaio](https://sites.google.com/view/leobino){:target="\_blank"} in the [INSERT Research Group](https://insert-lab.netlify.app){:target="\_blank"}. Where I also received an M.Sc. degree in Computer Science in July 2018.

My research during my M.Sc. focused on mobility support in wireless environments of Named Data Networking (NDN) networks. Currently, my research interests include secure and efficient packet forwarding at the edge of NDN architecture.

Before that, I received a B.S. degree in Computer Networks from the [Federal University of Ceará](https://www.quixada.ufc.br){:target="\_blank"} in December 2014. During my undergraduate years, I was advised by [Prof. Paulo Rego](https://cc.ufc.br/curso/corpo-docente/pauloalr){:target="\_blank"}. My research during this time focused on opportunistic private clouds.

More information, in my [Lattes curriculum](http://lattes.cnpq.br/3102385411862897){:target="\_blank"} in Portuguese.

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
