---
permalink: /publications/
title: "Publications and preprints"
---

<!-- The list below is generated from _data/publications.yml — edit that file to add papers (newest at the top). -->

<ol class="pub-list">
{% for p in site.data.publications %}
  <li class="pub-entry">
    <span class="pub-title">{{ p.title }}</span><br>
    <span class="pub-authors">{{ p.authors | markdownify | remove: '<p>' | remove: '</p>' | strip }}</span><br>
    <em>{{ p.venue }}</em>{% if p.details %}, {{ p.details }}{% endif %}{% if p.status %} ({{ p.status }}){% endif %}, {{ p.year }}.{% if p.note %} <span class="pub-note">{{ p.note }}</span>{% endif %}
    <span class="pub-links">
      {% if p.arxiv %}[<a href="https://arxiv.org/abs/{{ p.arxiv }}">arXiv</a>] {% endif %}
      {% if p.doi %}[<a href="https://doi.org/{{ p.doi }}">DOI</a>] {% endif %}
      {% if p.url %}[<a href="{{ p.url }}">Link</a>] {% endif %}
      {% if p.pdf %}[<a href="{{ p.pdf }}">PDF</a>] {% endif %}
    </span>
  </li>
{% endfor %}
</ol>
