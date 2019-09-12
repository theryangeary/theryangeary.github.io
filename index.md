# Portfolio

<div style="width: 100%; overflow: hidden">
{% for i in (0..site.projects.size) %}

  {% assign x = i %}
  <div style="float: left; padding: 10px">
    <h2>
      <a href="{{ site.projects[x].project-url }}">{{ site.projects[x].title }}</a>
    </h2>

    <p>
      {{ site.projects[x].content }}
    </p>
  </div>

{% endfor %}
</div>
