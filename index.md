---
title: Hello, World!
layout: default
---

# hello world!

{% for exp in site.experiments %}
<div class="panel panel-default">
  <div class="panel-heading">{{ exp.title }}</div>
  <div class="panel-body">
    <p> {{ exp.description }} </p>
    <a href="{{ exp.url }}" class="btn btn-default">Start Experiment</a>
  </div>
</div>
{% endfor %}
