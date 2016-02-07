---
layout: default
align: left
weight: 1
---

{% for post in site.posts limit: 5 %}

<h2>The latest from the Snell lab</h2>

<div class="row-fluid">
  <div class="span12">
    <h4>{{ post.date | date: "%B %d %Y" }}: {{ post.title }}</h4>
    <p>{{ post.content }}</p>
  </div>
</div>
<br/>

{% endfor %}
