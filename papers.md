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
            <b>{{ p[1].title }}</b>
            <br>
            <i>{{ p[1].authors }}</i>
            <!-- {% if p[1].alt_url == "" %} -->
              <!-- (<a href="{{ site.baseurl }}/papers/KR2ML_2020_{{ p[0] }}.pdf">PDF</a>) -->
            <!-- {% elsif p[1].alt_url == "NONE" %} -->
              <!-- (PDF not available) -->
            <!-- {% else %} -->
              <!-- (<a href="{{ p[1].alt_url }}">PDF</a>) -->
            <!-- {% endif %} -->
        </li>
    {% endfor %}
  </ol>
</div>
