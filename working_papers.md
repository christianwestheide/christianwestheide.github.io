---
layout: page
permalink: /working_papers/
title: Working Papers
---

<ul class="listing">
{% for item in site.data.working_papers %}
	<li>
		<b>{{item.title}}</b><br/>
		{{item.authors}}, {{item.year}}<br/>
		<div class="link-buttons">
			{% if item.abstract %}
				<details>
	 			<summary class="color-button2" >Show Abstract</summary> <!--  -->
				<p class="abstract-open">{{item.abstract}}</p>
				</details>
			{% endif %}
			{% if item.ssrn %}
					<a href ="{{item.ssrn}}" target ="_blank"><div class = "color-button2">Paper</div></a>
			{% else %}
			  &nbsp;
			{% endif %}
		</div>
		<br/>
	</li>
{% endfor %}
</ul>
