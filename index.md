---
title: Hello, World!
layout: default
---

# hello world!

{% for exp in site.experiments %}
<div class="panel panel-default">
  <div class="panel-heading">{{ experiment.title }}</div>
  <div class="panel-body">
    <p> {{ experiment.description }} </p>
    <a href="{{ experiment.url }}" class="btn btn-default">Start Experiment</a>
  </div>
</div>
{% endfor %}
