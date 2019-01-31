# Portfolio

<div style="width: 100%; overflow: hidden">
{% for i in (0..site.projects.size) %}

  {% assign x = i | times:2 %}
  <div style="float: left; width: 50%; padding: 10px">
    <h2>
      <a href="{{ site.projects[x].project-url }}">{{ site.projects[x].title }}</a>
    </h2>

    <p>
      {{ site.projects[x].content }}
    </p>
  </div>

  {% assign x = x | plus:1 %}
  <div style="float: right; width: 50%; padding: 10px">
    <h2>
      <a href="{{ site.projects[x].project-url }}">{{ site.projects[x].title }}</a>
    </h2>

    <p>
      {{ site.projects[x].content }}
    </p>
  </div>

{% endfor %}
</div>
