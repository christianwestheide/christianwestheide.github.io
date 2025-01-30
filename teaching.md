---
layout: page
title: Teaching
permalink: /teaching/
---
<h2>Current teaching</h2>
<ul class="listing">
{% for item in site.data.teaching %}
{% if item.current>0 %}
	<li>
		<b>{{item.title}}</b><br/>
    {% if item.description %}
		{{item.description}}
    <br/>
		{% endif %}
		{{item.schedule}}<br/>
    {% if item.link %}
		<div class="link-buttons">
    <a href ="{{item.link}}" target ="_blank"><div class = "color-button2">Course Description</div></a>
		</div>
    {% endif %}
		<br/>
	</li>
{% endif %}  
{% endfor %}
</ul>
<h2>Past teaching</h2>

<ul class="listing">
{% for item in site.data.teaching %}
{% if item.current==0 %}
	<li>
		<b>{{item.title}}</b><br/>
    {% if item.description %}
		{{item.description}}
    <br/>
		{% endif %}
		{{item.schedule}}<br/>
    {% if item.link %}
		<div class="link-buttons">
    <a href ="{{item.link}}" target ="_blank"><div class = "color-button2">Course Description</div></a>
		</div>
    {% endif %}
		<br/>
	</li>
  {% endif %}
{% endfor %}
</ul>
