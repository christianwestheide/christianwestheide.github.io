---
layout: page
permalink: /publications/
title: Publications
---
<ul class="listing">
{% for item in site.data.publications %}
	<li>
		<b>{{item.title}}</b><br/>
		{{item.authors}}<br/>
    {{item.journal}}<br/>
		<div class="link-buttons">

		{% if item.abstract %}
		<details >
	 	<summary class="color-button2" >Show Abstract</summary>
		<p class="abstract-open">{{item.abstract}}</p>
		</details>
		{% endif %}
		{% if item.doi %}

		<a href ="{{item.doi}}" target ="_blank">&nbsp;<div class = "color-button2">Journal Article</div></a>
		{% endif %}
		{% if item.ssrn %}
		<a href ="{{item.ssrn}}" target ="_blank">
		<div class = "color-button2">Working Paper Version</div></a>
		{% endif %}
		</div>
		<br/>
	</li>
{% endfor %}
</ul>
{{page.url}}
