---
layout: page
title: KR2ML
subtitle: Knowledge Representation & Reasoning Meets Machine Learning
use-site-title: true
---

# About

Machine learning (ML) has seen a tremendous amount of recent success and has been applied in a variety of applications. However, it comes with several drawbacks, such as the need for large amounts of training data and the lack of explainability and verifiability of the results. In many domains, there is structured knowledge (e.g., from electronic health records, laws, clinical guidelines, or common sense knowledge) which can be leveraged for reasoning in an informed way (i.e., including the information encoded in the knowledge representation itself) in order to obtain high quality answers. Symbolic approaches for knowledge representation and reasoning (KR) are less prominent today - mainly due to their lack of scalability - but their strength lies in the verifiable and interpretable reasoning that can be accomplished. This workshop aims at the intersection of these two sub-fields of AI, and hopes to shine a light on the synergies that exist between KR and ML.

To reach a broader audience and increase the public awareness of the importance of the topic, we propose to hold the second KR2ML workshop at NeurIPS 2019. Our goal is to advance the general discussion of the topic by highlighting contributions that propose innovative approaches integrating KR and ML (i.e., in contrast to approaches that just augment previous work in "established" areas of interaction, such as knowledge graph embeddings). Moreover, we will have a call for key challenges, which will be presented and discussed in a special session at the workshop, and later released as a special report for the field to consider. Our tentative list of invited speakers/panel covers renown experts from both academia and industry who have made important contributions to the integration of KR and ML across a spectrum of approaches to combining the fields. The program (a tentative schedule is attached below) will be rounded off by a poster session, which will provide the time and space for preliminary ideas to be discussed.

# Program

The focus of KR2ML is to initiate and continue discussions and collaborations between researchers from the two umbrella areas- KRR and ML. To encourage this interaction, the program features several invited talks of experienced researchers about challenges in the field as well as successful work in the area. A special key challenge session invites open discussion of major problems and opportunities. Some of the problems will be further highlighted in a discussion panel of prominent experts,  which will also give attendees the opportunity to contribute.  Finally, poster sessions throughout the day will provide room for presenting and discussing ongoing works and exploring possible collaborations; they will bestarted by one-minute spotlight talks highlighting the posters. We hope to attract many participants and will use a plenary format for the talks.

# Speakers

- William W. Cohen (Accepted)
- Xin Luna Dong (Accepted)
- Oren Etzioni (Accepted)
- Francesca Rossi (Accepted)
- Michael Witbrock (Accepted)

# Organizers

- [Veronika Thost](https://researcher.watson.ibm.com/researcher/view.php?person=ibm-Veronika.Thost)
- [Christian Muise](http://www.haz.ca/)
- [Kartik Talamadupula](http://www.ktalamad.com/)
- [Sameer Singh](http://www.sameersingh.org/)
- [Christopher Ré](https://cs.stanford.edu/people/chrismre/)

<!-- <div class="posts-list">
  {% for post in paginator.posts %}
  <article class="post-preview">
    <a href="{{ post.url | prepend: site.baseurl }}">
	  <h2 class="post-title">{{ post.title }}</h2>

	  {% if post.subtitle %}
	  <h3 class="post-subtitle">
	    {{ post.subtitle }}
	  </h3>
	  {% endif %}
    </a>

    <p class="post-meta">
      Posted on {{ post.date | date: "%B %-d, %Y" }}
    </p>

    <div class="post-entry-container">
      {% if post.image %}
      <div class="post-image">
        <a href="{{ post.url | prepend: site.baseurl }}">
          <img src="{{ post.image }}">
        </a>
      </div>
      {% endif %}
      <div class="post-entry">
        {{ post.excerpt | strip_html | xml_escape | truncatewords: site.excerpt_length }}
        {% assign excerpt_word_count = post.excerpt | number_of_words %}
        {% if post.content != post.excerpt or excerpt_word_count > site.excerpt_length %}
          <a href="{{ post.url | prepend: site.baseurl }}" class="post-read-more">[Read&nbsp;More]</a>
        {% endif %}
      </div>
    </div>

    {% if post.tags.size > 0 %}
    <div class="blog-tags">
      Tags:
      {% if site.link-tags %}
      {% for tag in post.tags %}
      <a href="{{ site.baseurl }}/tags#{{- tag -}}">{{- tag -}}</a>
      {% endfor %}
      {% else %}
        {{ post.tags | join: ", " }}
      {% endif %}
    </div>
    {% endif %}

   </article>
  {% endfor %}
</div>

{% if paginator.total_pages > 1 %}
<ul class="pager main-pager">
  {% if paginator.previous_page %}
  <li class="previous">
    <a href="{{ paginator.previous_page_path | prepend: site.baseurl | replace: '//', '/' }}">&larr; Newer Posts</a>
  </li>
  {% endif %}
  {% if paginator.next_page %}
  <li class="next">
    <a href="{{ paginator.next_page_path | prepend: site.baseurl | replace: '//', '/' }}">Older Posts &rarr;</a>
  </li>
  {% endif %}
</ul>
{% endif %} -->
