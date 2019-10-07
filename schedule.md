---
layout: page
title: KR2ML
subtitle: Knowledge Representation & Reasoning Meets Machine Learning
use-site-title: true
---

# Schedule

<div class="container">
  <div class="row">
    <table class="table">
        {% for s in site.data.schedule %}
        <tr>
        <td>{{ s[1].start }}</td>
        {% if s[1].type == "General" %}
          <td>{{ s[1].event }}</td>
          <td></td>
        {% elsif s[1].type == "Invited" %}
          <td class="success"><b>Invited Talk</b></td>
          {% assign speaker_id = s[1].event %}
          {% assign speaker = site.data.speakers[speaker_id] %}
          <td class="success"><a href="{{speaker.url}}">{{ speaker.name }}</a>, {{speaker.affiliation}}</td>
        {% elsif s[1].type == "Contributed" %}
          <td><i>Contributed Talk</i></td>
          <td></td>
        {% elsif s[1].type == "Spotlights" %}
          <td>Spotlights</td>
          <td>{{ s[1].event }}</td>
        {% elsif s[1].type == "Break" %}
          <td class="info"></td>
          <td class="info">{{ s[1].event }}</td>
        {% endif %}

        <!-- <td>
            {% capture id %}{{ p[0] }}{% endcapture %}
            {{ s }}
        </td> -->
        </tr>
        {% endfor %}
    </table>
  </div>
</div>
