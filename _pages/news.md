---
layout: archive
title: "News"
permalink: /news/
author_profile: true
---

{% include base_path %}

<div class="news-archive">
  {% assign sorted_news = site.news | sort: 'date' | reverse %}
  {% for news_item in sorted_news %}
    <div class="news-item-full">
      <h3><a href="{{ base_path }}{{ news_item.url }}">{{ news_item.title }}</a></h3>
      <span class="news-date-full">{{ news_item.date | date: "%B %d, %Y" }}</span>
      <p>{{ news_item.content | strip_html | truncatewords: 50 }}</p>
      <a href="{{ base_path }}{{ news_item.url }}" class="read-more">Read more →</a>
    </div>
  {% endfor %}
</div>
