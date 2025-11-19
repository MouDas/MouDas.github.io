---
layout: home
title: "Welcome to My Blog"
---

# Welcome to My Blog!

This blog tracks my progress building a **Meal Planner app**.

Here you will find:

- Daily updates on my project
- Notes on Git, GitHub, and VS Code
- Steps to build the Meal Planner app

---

## Recent Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%B %d, %Y" }}
    </li>
  {% endfor %}
</ul>

---

Happy blogging! 📝

