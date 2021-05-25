{% include breadcrumbs.html %}
<h1>Jobs listing:</h1>
{% for job in site.jobs %}
  <h2>
    <a href="/jobs/{{ job.url }}">
      {{ job.title }}
    </a>
  </h2>
  <p>{{ job.description | markdownify }}</p>
{% endfor %}