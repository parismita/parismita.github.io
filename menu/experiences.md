---
layout: default
title: Home
---

{% for post in site.posts %}
<div class="posts">
  {% if post.title == "Experience!" %}
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

<!-- Pagination links -->
<div class="pagination">
  {% if paginator.next_page %}
    <a class="pagination-button pagination-active" href="{{ site.github.url }}{{ paginator.next_page_path }}" class="next">{{ site.data.settings.pagination.previous_page }}</a>
  {% else %}
    <span class="pagination-button">{{ site.data.settings.pagination.previous_page }}</span>
  {% endif %}

  {% if paginator.previous_page %}
    <a class="pagination-button pagination-active" href="{{ site.baseurl }}{{ paginator.previous_page_path }}">{{ site.data.settings.pagination.next_page }}</a>
  {% else %}
    <span class="pagination-button">{{ site.data.settings.pagination.next_page }}</span>
  {% endif %}
</div>
