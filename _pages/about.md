---
permalink: /
title: " "
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

I am a Senior ML Research Engineer at the Kempner Institute at Harvard, specializing in performance and efficiency in machine learning. My work spans large-scale experiments on diffusion models and transformers, performance benchmarking on GPU clusters, and the development of reproducible open-source codebases. I focus on rapidly implementing research ideas, profiling and optimizing bottlenecks, and delivering systems that make AI experiments faster, scalable, and reliable.

## Schedule a Meeting

Interested in collaboration or discussing research or potential collaboration opportunities? I'm always open to connecting with fellow researchers, students, and industry professionals.

<div style="text-align: center; margin: 20px 0;">
  <a href="https://calendar.app.google/jky14xruQdbihX4c9" target="_blank" style="background-color: #146bf8ff; color: white; padding: 8px 16px; text-decoration: none; border-radius: 4px; display: inline-block; font-size: 0.9em;"> Book an Appointment</a>
</div>

<div class="news-container">
  <h2>Recent News</h2>
  {% assign sorted_news = site.news | sort: 'date' | reverse %}
  {% for news_item in sorted_news limit: 10 %}
    <div class="news-item">
      <span class="news-date">{{ news_item.date | date: "%b %Y" }}</span>
      <a href="{{ news_item.url | relative_url }}" class="news-title-link">{{ news_item.title }}</a>
    </div>
  {% endfor %}
  <p><a href="{{ '/news/' | relative_url }}" class="view-all-news">View all news →</a></p>
</div>
