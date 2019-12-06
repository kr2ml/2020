---
layout: page
title: KR2ML
subtitle: Knowledge Representation & Reasoning Meets Machine Learning
use-site-title: true
---

## Friday, December 13, 2019

## Location: West 109 + 110, Area West Level 1

# About

Machine learning (ML) has seen a tremendous amount of recent success and has been applied in a variety of applications. However, it comes with several drawbacks, such as the need for large amounts of training data and the lack of explainability and verifiability of the results. In many domains, there is structured knowledge (e.g., from electronic health records, laws, clinical guidelines, or common sense knowledge) which can be leveraged for reasoning in an informed way (i.e., including the information encoded in the knowledge representation itself) in order to obtain high quality answers. Symbolic approaches for knowledge representation and reasoning (KR) are less prominent today - mainly due to their lack of scalability - but their strength lies in the verifiable and interpretable reasoning that can be accomplished. This workshop aims at the intersection of these two sub-fields of AI, and hopes to shine a light on the synergies that exist between KR and ML.

To reach a broader audience and increase the public awareness of the importance of the topic, we propose to hold the second KR2ML workshop at NeurIPS 2019. Our goal is to advance the general discussion of the topic by highlighting contributions that propose innovative approaches integrating KR and ML (i.e., in contrast to approaches that just augment previous work in "established" areas of interaction, such as knowledge graph embeddings). Moreover, we will have a call for key challenges, which will be presented and discussed in a special session at the workshop, and later released as a special report for the field to consider. Our tentative list of invited speakers/panel covers renown experts from both academia and industry who have made important contributions to the integration of KR and ML across a spectrum of approaches to combining the fields. The program will be rounded off by a poster session, which will provide the time and space for preliminary ideas to be discussed.

<!--

# Program

The focus of KR2ML is to initiate and continue discussions and collaborations between researchers from the two umbrella areas- KRR and ML. To encourage this interaction, the program features several invited talks of experienced researchers about challenges in the field as well as successful work in the area. A special key challenge session invites open discussion of major problems and opportunities. Some of the problems will be further highlighted in a discussion panel of prominent experts, which will also give attendees the opportunity to contribute. Finally, poster sessions throughout the day will provide room for presenting and discussing ongoing works and exploring possible collaborations; they will bestarted by one-minute spotlight talks highlighting the posters. We hope to attract many participants and will use a plenary format for the talks.
-->

# Speakers

<div class="container">
  <div class="row">
  {% for p in site.data.speakers %}
  {% capture id %}{{ p[0] }}{% endcapture %}
  {% unless p[0] == "tba" %}
  {% include profile.html p=p %}
  {% endunless %}
  {% endfor %}
  </div>
</div>

# Important Dates 


{% include dates.md %}

# Organizers

<!-- prettier-ignore -->
<div class="container">
  <div class="row">
    {% for p in site.data.organizers %}
    {% capture id %}{{ p[0] }}{% endcapture %}
    {% include profile.html p=p %}
    {% endfor %}
  </div>
</div>

# Related Venues

- [Workshop on Neural-Symbolic Learning and Reasoning (NeSys'19)](https://sites.google.com/view/nesy2019/home), see more on <http://www.neural-symbolic.org/>
- [Workshop on Semantic Deep Learning (SemDeep'19)](http://www.dfki.de/semdeep-5/)
- [Workshop on Deep Learning for Knowledge Graphs (DL4KG'19)](https://alammehwish.github.io/dl4kg-eswc/)
- [Workshop on Semantic Explainability (SEMEX'19)](http://www.semantic-explainability.com/)
- [Workshop on Statistical Relational AI (StarAI'18)](http://www.starai.org/2018/)
- [Automated Knowledge Base Construction (AKBC'19)](http://www.akbc.ws/2019/)

Contact: <kr2ml.ws@gmail.com>.
