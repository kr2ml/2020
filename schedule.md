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
          {% assign paper_id = s[1].event %}
          {% assign paper = site.data.papers[paper_id] %}
          <td>
            {{ paper.authors }}<br>
            <i>{{ paper.title }}</i>
            {% if paper.alt_url == "" %}
              (<a href="{{ site.baseurl }}/papers/KR2ML_2019_{{ paper_id }}.pdf">PDF</a>)
            {% elsif paper.alt_url == "NONE" %}
            {% else %}
              (<a href="{{ paper.alt_url }}">PDF</a>)
            {% endif %}
          </td>
        {% elsif s[1].type == "Spotlights" %}
          <td>Spotlights</td>
          <td><a href="#{{s[0]}}">{{ s[1].event }}</a></td>
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

<h1 id="spotlightsA"> Spotlights A </h1>

  {% assign spotlightApapers = "paper_1, paper_2, paper_3, paper_5, paper_6, paper_8, paper_11, paper_12, paper_17, paper_21, paper_22, paper_23, paper_26, paper_27, paper_28, paper_29, paper_30, paper_31, paper_33, paper_34, paper_36, paper_37, paper_38" | split: ", " %}

  <div class="row">
    <ol>
      {% for p in spotlightApapers %}
        <li>
            {% assign paper = site.data.papers[p] %}
            <b>{{ paper.authors }}</b>.
            <i>{{ paper.title }}</i>
            {% if paper.alt_url == "" %}
              (<a href="{{ site.baseurl }}/papers/KR2ML_2019_{{ paper_id }}.pdf">PDF</a>)
            {% elsif paper.alt_url == "NONE" %}
            {% else %}
              (<a href="{{ paper.alt_url }}">PDF</a>)
            {% endif %}
        </li>
      {% endfor %}
    </ol>
  </div>

<h1 id="spotlightsB"> Spotlights B </h1>

  {% assign spotlightBpapers = "paper_39, paper_40, paper_42, paper_43, paper_44, paper_46, paper_50, paper_54, paper_55, paper_56, paper_57, paper_58, paper_59, paper_62" | split: ", " %}
  <div class="row">
    <ol>
      {% for p in spotlightBpapers %}
        <li>
            {% assign paper = site.data.papers[p] %}
            <b>{{ paper.authors }}</b>.
            <i>{{ paper.title }}</i>
            {% if paper.alt_url == "" %}
              (<a href="{{ site.baseurl }}/papers/KR2ML_2019_{{ paper_id }}.pdf">PDF</a>)
            {% elsif paper.alt_url == "NONE" %}
            {% else %}
              (<a href="{{ paper.alt_url }}">PDF</a>)
            {% endif %}
        </li>
      {% endfor %}
    </ol>
  </div>

</div>
