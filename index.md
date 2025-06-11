---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
---
layout: home
title: "James Ndarila"
author_profile: true
---

## Welcome!

Hi, I’m **James Ndarila** — an ICT specialist and Data Enthusiast passionate about digital literacy, analytics, and empowering communities with technology.

Currently advancing my skills in data and AI through the Cyber Shujaa Programme. Check out my work and feel free to connect!

📄 [Download My Resume (PDF)](/assets/files/James-Ndarila-CV.pdf)

---

## 🔧 Featured Projects

- **Hotel Dashboard** – Power BI project for hotel business insights.
- **Netflix Analysis** – Cleaned and visualized Netflix dataset with Python.
- **Titanic EDA** – Performed exploratory data analysis on Titanic dataset.

---

## 📝 Latest Posts

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url | relative_url }}) – {{ post.date | date: "%B %d, %Y" }}
{% endfor %}
