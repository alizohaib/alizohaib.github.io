<h4 id="projects">Projects/Tools</h4>

<div class="projects-list">
{% for item in site.data.projects.main %}
  <div class="project-entry">
    <div class="project-name">
      {% if item.link %}<a href="{{ item.link }}" target="_blank" rel="noopener">{{ item.name }}</a>{% else %}{{ item.name }}{% endif %}
    </div>
    <div class="project-description">{{ item.description }}</div>
  </div>
{% endfor %}
</div>
