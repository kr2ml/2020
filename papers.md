---
layout: page
title: KR2ML
subtitle: Knowledge Representation & Reasoning Meets Machine Learning
use-site-title: true
---

# Accepted Papers

<div class="container">
  <ol>
    {% for p in site.data.papers %}
        <li id="{{ p[0] }}">
            <b>{{ p[1].authors }}</b>.
            <i>{{ p[1].title }}</i>
            (<a href="{{ site.baseurl }}/papers/KR2ML_2019_{{ p[0] }}.pdf">PDF</a>)
        </li>
    {% endfor %}
  </ol>
</div>