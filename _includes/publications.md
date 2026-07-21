<h4 id="publications">Publications</h4>

<div class="publications-list">
{% for link in site.data.publications.main %}
  <div class="pub-entry">
    <div class="pub-title">
      {% if link.pdf %}<a href="{{ link.pdf }}" target="_blank" rel="noopener">{{ link.title }}</a>{% else %}{{ link.title }}{% endif %}
    </div>
    <div class="pub-authors">{{ link.authors }}</div>
    <div class="pub-venue"><em>{{ link.conference }}</em>{% if link.year %}, {{ link.year }}{% endif %}</div>
    {% if link.notes %}
    <div class="pub-notes"><strong>{{ link.notes | strip | newline_to_br }}</strong></div>
    {% endif %}
  </div>
{% endfor %}
</div>
