---
layout: page
title: "Projects!"
author: "Parismita Das"
categories: journal
tags: [documentation,sample]
image: stool.jpg
---

## Projects

<div class="posts">
  <h1>
    <a href="https://aldro61.github.io/mmit/tutorials/R/">MMIT</a>
  </h1>
  
  <div class="thumbnail-container">
    <a href="https://aldro61.github.io/mmit/tutorials/R/"><img src=""></a>
  </div>
  
  <p>
    There are few R packages available for interval regression, a machine learning problem which is important in genomics and medicine. Like usual regression, the goal is to learn a function that inputs a feature vector and outputs a real-valued prediction. Unlike usual regression, each response in the training set is an interval of acceptable values (rather than one value). In the terminology of the survival analysis literature, this is regression with “left, right, and interval censored” output/response data.
  </p>
 </div>


{% for post in site.posts %}
 <div class="posts">
  {% if post.title == "Project!" %}
  <h1>
    <a href="{{ site.github.url }}{{ post.url }}">{{ post.title2 }}</a>
  </h1>
  
  <div class="thumbnail-container">
    <a href="{{ site.github.url }}{{ post.url }}"><img src="{{ site.github.url }}/assets/img/{{ post.image }}"></a>
  </div>
  
  <p>
    {{ post.content | strip_html | truncate: 350 }} <a href="{{ site.github.url }}{{ post.url }}">Read more</a>
    <span class="post-date"> <i class="fa fa-clock-o" aria-hidden="true"></i> {% include read-time.html %}</span>
  </p>
 </div>
  {% endif %}
{% endfor %}

[Home Automation](https://www.instructables.com/id/Making-Smart-home-Devices-techiniche-boltiot/)



