---
layout: default
title: Achievements
permalink: /achievements/
---
<h2>Achievements</h2>
<ul>
{% assign items = site.achievements | sort: "date" | reverse %}
{% for item in items %}
<li><a href="{{ item.url }}">{{ item.title }}</a> — {{ item.date | date: "%b %Y" }}</li>
{% endfor %}
</ul>
