<h1>Jobs listing:</h1>
{% for job in site.jobs %}
  <h2>
    <a href="{{ job.url }}">
      {{ job.name }} - {{ job.position }}
    </a>
  </h2>
  <p>{{ job.content | markdownify }}</p>
{% endfor %}