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

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
1. Hipótesis lineales sobre medias para experimentos de franjas en parcelas divididas.

* Departamento de Estadística, Universidad Nacional de Colombia, Bogotá, 2004. Undergraduate dissertation (Spanish). [pdf](https://danielandresgp.github.io/files/TesisPregrado.pdf).

