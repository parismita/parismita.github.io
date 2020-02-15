---
layout: default
title: Home
---

<div class="posts2">
  <h1>
    <a href="https://parismita.github.io/assets/tutorial">MMIT</a>
  </h1>
  
  <div class="thumbnail-container">
    <a href="https://parismita.github.io/assets/tutorial"><img src="https://ai2-s2-public.s3.amazonaws.com/figures/2017-08-08/c0c4573cb8bc9c03815c664aeeaebb99ae237040/3-Figure1-1.png"></a>
  </div>
  
  <p> 
    There are few R packages available for interval regression, a machine learning problem which is important in genomics and medicine. Like usual regression, the goal is to learn a function that inputs a feature vector and outputs a real-valued prediction...<a href="https://parismita.github.io/assets/tutorial">Read more</a><span class="post-date"> <i class="fa fa-clock-o" aria-hidden="true"></i> {% include read-time.html %}</span>
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


<div class="posts3">
  <h1>
    <a href="https://www.instructables.com/id/Making-Smart-home-Devices-techiniche-boltiot/">Home Automation</a>
  </h1>
  
  <div class="thumbnail-container">
    <a href="https://www.instructables.com/id/Making-Smart-home-Devices-techiniche-boltiot/"><img src="https://cdn.instructables.com/FDR/UT8B/IMTGE6ID/FDRUT8BIMTGE6ID.LARGE.jpg?auto=webp&fit=bounds"></a>
  </div>
  
  <p> 
    The idea of this project is to detect whenever a person leaves a room empty and if the fans or lights are on then he will get a ping on his smartphone through an app . Also, the lights and fans can be switched off by using the app itself rather than going back inside the room...<a href="https://www.instructables.com/id/Making-Smart-home-Devices-techiniche-boltiot/">Read more</a><span class="post-date"> <i class="fa fa-clock-o" aria-hidden="true"></i> {% include read-time.html %}</span>
  </p>
 </div>




