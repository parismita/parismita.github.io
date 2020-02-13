---
layout: default
title: Home
---

<div class="posts2">
  <h1>
    <a href="https://aldro61.github.io/mmit/tutorials/R/">MMIT</a>
  </h1>
  
  <div class="thumbnail-container">
    <a href="https://aldro61.github.io/mmit/tutorials/R/"><img src=""></a>
  </div>
  
  <p> 
    There are few R packages available for interval regression, a machine learning problem which is important in genomics and medicine. Like usual regression, the goal is to learn a function that inputs a feature vector and outputs a real-valued prediction...<a href="https://aldro61.github.io/mmit/tutorials/R/">Read more</a><span class="post-date"> <i class="fa fa-clock-o" aria-hidden="true"></i> {% include read-time.html %}</span>
  </p>
 </div>
</br>

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




