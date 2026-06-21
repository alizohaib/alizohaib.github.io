<h4 id="highlights">Highlights</h4>

<ul class="news-list">
{% assign sorted_news = site.data.news.main | sort: "sort_date" | reverse %}
{% for item in sorted_news limit: 10 %}
  <li class="news-item">
    <span class="news-date">{{ item.date }}</span>
    <span class="news-sep">&mdash;</span>
    <span class="news-content">{{ item.content }}</span>
  </li>
{% endfor %}
</ul>
