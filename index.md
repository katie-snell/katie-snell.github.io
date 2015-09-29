---
layout: default
menu: Sausage
icon: home
align: left
weight: 1
---

{% for post in site.posts limit: 5 %}

<div class="row-fluid">
  <div class="span12">
    <h2>{{ post.title }}</h2>
    <h4>{{ post.date | date_to_long_string }}</h4>
    <p>{{ post.content }}</p>
  </div>
</div>
<br/>

{% endfor %}
