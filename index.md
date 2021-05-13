<span>Jobs listing:</span>
<ul>
    {% for job in site.data.jobs %}
    <li>
        <h2>Title: {{ job.title }}</h2>
        <p>Description: {{ job.description }}</p>
        <span>Published: {{ job.published }}</span>
    </li>
    {% endfor %}    
</ul>