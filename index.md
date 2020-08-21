---
layout: page
title: KR2ML
subtitle: Knowledge Representation & Reasoning Meets Machine Learning
use-site-title: true
---

<br />
<div class="sharethis-inline-share-buttons"></div>

# Overview

Machine learning (ML) has seen a tremendous amount of recent success and has been applied in a variety of applications. However, it comes with several drawbacks, such as the need for large amounts of training data and the lack of explainability and verifiability of the results. In many domains, there is structured knowledge (e.g., from electronic health records, laws, clinical guidelines, or common sense knowledge) which can be leveraged for reasoning in an informed way (i.e., including the information encoded in the knowledge representation itself) in order to obtain high quality answers. Symbolic approaches for knowledge representation and reasoning (KR) are less prominent today - mainly due to their lack of scalability - but their strength lies in the verifiable and interpretable reasoning that can be accomplished. This workshop aims at the intersection of these two sub-fields of AI, and hopes to shine a light on the synergies that exist between KRR and ML. The 4th KR2ML workshop will be a [virtual workshop at NeurIPS 2020](https://nips.cc/Conferences/2020/Schedule?showEvent=16122), December 11/12 (tbd). Our goal is to advance the general discussion of the topic by highlighting contributions proposing innovative approaches integrating KRR and ML.

<div class="container" style="margin-bottom: 10px;"></div>
<!--

# Program

The focus of KR2ML is to initiate and continue discussions and collaborations between researchers from the two umbrella areas- KRR and ML. To encourage this interaction, the program features several invited talks of experienced researchers about challenges in the field as well as successful work in the area. A special key challenge session invites open discussion of major problems and opportunities. Some of the problems will be further highlighted in a discussion panel of prominent experts, which will also give attendees the opportunity to contribute. Finally, poster sessions throughout the day will provide room for presenting and discussing ongoing works and exploring possible collaborations; they will bestarted by one-minute spotlight talks highlighting the posters. We hope to attract many participants and will use a plenary format for the talks.
-->

<hr>

# Speakers
<meta name="thumbnail" content="./img/neurips-logo-new.jpg" />

<div class="container" style="margin-top: 25px;margin-bottom: 20px;">
  <div class="row">
  {% for p in site.data.speakers %}
  {% capture id %}{{ p[0] }}{% endcapture %}
  {% include profile.html p=p %}
  {% endfor %}
  </div>
</div>

<!--
# Important Dates 

{% include dates.md %} 
-->

<hr>

# Organizers

<!-- prettier-ignore -->
<div class="container" style="margin-top: 25px;margin-bottom: 20px;">
  <div class="row">
    {% for p in site.data.organizers %}
    {% capture id %}{{ p[0] }}{% endcapture %}
    {% include profile.html p=p %}
    {% endfor %}
  </div>
</div>

<hr>

# Program Committee
TBD

<hr>

# Related Venues

<div class="container" style="margin-bottom: 10px;"></div>

- [Automated Knowledge Base Construction (AKBC'20)](http://www.akbc.ws/2020/)
- [Workshop on Semantic Deep Learning (SemDeep'20)](http://www.dfki.de/~declerck/semdeep-6/)
- [Workshop on Deep Learning for Knowledge Graphs (DL4KG'20)](https://alammehwish.github.io/dl4kg_eswc_2020/)
- [Workshop on Semantic Explainability (SEMEX'20)](http://www.semantic-explainability.com/)
- [Workshop on Statistical Relational AI (StarAI'20)](http://www.starai.org/2020/)
- [Workshop on Neural-Symbolic Learning and Reasoning (NeSys'19)](https://sites.google.com/view/nesy2019/home), see more on <http://www.neural-symbolic.org/>

<div class="container" style="margin-bottom: 10px;"></div>

<hr>

Contact: <kr2ml.ws@gmail.com>.
