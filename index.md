---
layout: home
title: "Welcome"
---

# Welcome to My Blog!

This blog will track my progress building a Meal Planner app.

- Suggests weekly lunch & dinner for a family of 4
- Avoids repeating recipes from the last 2 weeks
- Generates grocery lists and prep instructions

## Recent Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%B %d, %Y" }}
    </li>
  {% endfor %}
</ul>
