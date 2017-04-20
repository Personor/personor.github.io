---
layout: default
---

<body>
  <div class="index-wrapper">
    <div class="aside">
      <div class="info-card">
        <h1>Hebuny</h1>
		<div style="color:#F0FFFF"><p>Every light has darkness to balance it. </p></div>
      </div>
      <div id="particles-js"></div>
    </div>

    <div class="index-content">
      <ul class="artical-list">
        {% for post in site.categories.blog %}
        <li>
          <a href="{{ post.url }}" class="title">{{ post.title }}</a>
          <div class="title-desc">{{ post.description }}</div>
		  <div class="title-desc" style="font-size:12px">{{ post.author }} 发表于 {{ post.date | date: "%d %B %Y" }} </div>
        </li>
        {% endfor %}
      </ul>
    </div>
  </div>
</body>
