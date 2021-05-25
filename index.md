---
title: Jobs

---
<h1>Jobs listing:</h1>
<div  class="uk-margin uk-card uk-card-default uk-card-body">
{% for job in site.jobs %}
  <h2>
    <a href="{{ job.url }}">
      {{ job.title }}
    </a>
  </h2>
  <p>{{ job.description | markdownify }}</p>
  <p>Published on: {{ job.published  }}</p>
{% endfor %}
</div>