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
          <a href="{{ post.url }}" class="title" style="line-height:1.5">{{ post.title }}</a>
          <div class="title-desc">
			<img src="http://i.imgur.com/oMBcG88.jpg" style="width:100%;height:100%">
			{{ post.description }}
		  </div>
		  <div class="title-time">
			<span style="float:left">{{ post.author }} 发表于 {{ post.date | date: "%d %B %Y" }}</span> 
			<a href="{{ post.url }}" style="float:right">阅读全文</a>
		  </div>
        </li>
        {% endfor %}
      </ul>
    </div>
  </div>
</body>
