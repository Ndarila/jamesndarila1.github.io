---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
---
layout: home
title: "James Ndarila"
author_profile: true
---
<section>
  <h2>Welcome!</h2>
  <p>Hi, I’m <strong>James Ndarila</strong> — an ICT specialist and <strong>Data Enthusiast</strong> passionate about digital literacy, analytics, and empowering communities with technology.</p>

  <p>Currently advancing my skills in data and AI through the <strong>Cyber Shujaa Programme</strong>. Check out my work and feel free to connect!</p>

  <p>
    📄 <a href="/assets/files/James-Ndarila-CV.pdf" target="_blank" class="btn btn--primary">Download My Resume (PDF)</a>
  </p>
</section>

<section>
  <h2>Featured Projects</h2>
  <ul>
    <li><strong>Hotel Dashboard</strong> – Power BI project for hotel business insights.</li>
    <li><strong>Netflix Analysis</strong> – Cleaned and visualized Netflix dataset with Python.</li>
    <li><strong>Titanic EDA</strong> – Performed exploratory data analysis on Titanic dataset.</li>
  </ul>
</section>

<section>
  <h2>Latest Posts</h2>
  <ul>
    {% for post in site.posts limit:3 %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a><br />
        <small>{{ post.date | date: "%B %-d, %Y" }}</small><br />
        <p>{{ post.excerpt | strip_html | truncatewords: 25 }}</p>
      </li>
    {% endfor %}
  </ul>
  <a href="/blog/" class="btn btn--inverse">View All Posts</a>
</section>
