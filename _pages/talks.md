---
permalink: /talks/
title: "Talks"
---

<!-- Generated from _data/talks.yml — edit that file to add talks. -->

<ul class="talk-list">
{% for t in site.data.talks %}
  <li>
    <strong>{{ t.event }}</strong> — {{ t.place }}<br>
    <span class="talk-meta">{{ t.date }} · <em>{{ t.type }}</em>{% if t.video %} · [<a href="{{ t.video }}">video</a>]{% endif %}</span>
  </li>
{% endfor %}
</ul>
