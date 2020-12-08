---
layout: page
title: KR2ML
subtitle: Knowledge Representation & Reasoning Meets Machine Learning
use-site-title: true
---
<div class="sharethis-inline-share-buttons"></div>
<meta name="thumbnail" content="./img/neurips-logo-new.jpg" />

# Overview

Machine learning (ML) has seen a tremendous amount of recent success and has been applied in a variety of applications. However, it comes with several drawbacks, such as the need for large amounts of training data and the lack of explainability and verifiability of the results. In many domains, there is structured knowledge (e.g., from electronic health records, laws, clinical guidelines, or common sense knowledge) which can be leveraged for reasoning in an informed way (i.e., including the information encoded in the knowledge representation itself) in order to obtain high quality answers. Symbolic approaches for knowledge representation and reasoning (KRR) are less prominent today - mainly due to their lack of scalability - but their strength lies in the verifiable and interpretable reasoning that can be accomplished. This workshop aims at the intersection of these two sub-fields of AI, and hopes to shine a light on the synergies that exist between KRR and ML. The 4th KR2ML workshop will be a [virtual workshop at NeurIPS 2020](https://nips.cc/Conferences/2020/Schedule?showEvent=16122), Dec. 11. Our goal is to advance the general discussion of the topic by highlighting contributions proposing innovative approaches integrating KRR and ML.

<!-- | ------------- |:-------------:|
| **Submission** | October 09, 2020 (midnight Pacific Time) |
| **Notification** | October 30, 2020 |
| **Submission link**| [https://cmt3.research.microsoft.com/KR2ML2020](https://cmt3.research.microsoft.com/KR2ML2020) -->

* Thank you Amazon for sponsoring a best paper award!
* The 3 best papers will be presented in talks at the workshop! 
* <a href="schedule">The schedule is online now!</a> 
* <a href="papers">List of accepted papers available!</a> 
<!--* **NEW** Updates to existing submissions possible until October 12 (11:59pm Pacific Time) <br>New submissions close on October 09 (11:59pm Pacific Time)-->


<hr>

# Speakers & Panelists
<div class="container" style="margin-top: 20px;margin-bottom: 0px;">
  <div class="row">
  {% for p in site.data.speakers %}
  {% if forloop.index<=5 %}
  {% capture id %}{{ p[0] }}{% endcapture %}
  {% include profile.html p=p %}
  {% endif %}
  {% endfor %}
  </div>
  <div class="row">
  {% for p in site.data.speakers %}
  {% capture id %}{{ p[0] }}{% endcapture %}
  {% if forloop.index>5 and forloop.index<=10%}
  {% include profile.html p=p %}
  {% endif %}
  {% endfor %}
  </div>
  <div class="row">
  {% for p in site.data.speakers %}
  {% capture id %}{{ p[0] }}{% endcapture %}
  {% if forloop.index>10%}
  {% include profile.html p=p %}
  {% endif %}
  {% endfor %}
  </div>
<a href="speakers">More Info</a>
</div>

<hr>

# Organizers

<!-- prettier-ignore -->
<div class="container" style="margin-top: 25px;margin-bottom: 40px;">
  <div class="row">
    {% for p in site.data.organizers %}
    {% capture id %}{{ p[0] }}{% endcapture %}
    {% include profile.html p=p %}
    {% endfor %}
  </div>
</div>
<hr>

# Program Committee
<!-- prettier-ignore -->
<div class="container">
  <ul class="list-group list-group-flush">
    {% for p in site.data.pc.people %}
      <li class="list-group-item col-xs-6 col-sm-4 col-md-3">{{ p }}</li>
    {% endfor %}
  </ul>
</div>
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
