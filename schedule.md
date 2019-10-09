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
            <i>{{paper.authors}}</i><br>
            {{paper.title}} (<a href="{{site.baseurl}}/papers#{{paper_id}}">link</a>)</td>
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

  {% assign spotlightApapers = "paper2, paper3, paper6, paper8, paper11, paper12, paper17, paper21, paper22, paper23, paper26, paper27, paper28, paper29, paper31, paper34" | split: ", " %}
  <div class="row">
    <ol>
      {% for p in spotlightApapers %}
        <li>
            {% assign paper = site.data.papers[p] %}
            <i>{{paper.authors}}</i><br>
            {{paper.title}} (<a href="{{site.baseurl}}/papers#{{p}}">link</a>)
        </li>
      {% endfor %}
    </ol>
  </div>

<h1 id="spotlightsB"> Spotlights B </h1>

  {% assign spotlightBpapers = "paper36, paper37, paper38, paper39, paper40, paper42, paper43, paper44, paper46, paper54, paper55, paper56, paper57, paper58, paper59, paper62" | split: ", " %}
  <div class="row">
    <ol>
      {% for p in spotlightBpapers %}
        <li>
            {% assign paper = site.data.papers[p] %}
            <i>{{paper.authors}}</i><br>
            {{paper.title}} (<a href="{{site.baseurl}}/papers#{{p}}">link</a>)
        </li>
      {% endfor %}
    </ol>
  </div>


</div>
