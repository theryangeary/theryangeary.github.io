# Portfolio

{% for project in site.projects %}
## [{{ project.title }}]({{ project.project-url }})

{{ project.content }}

[Learn more]({{ project.project-url }})
{% endfor %}
