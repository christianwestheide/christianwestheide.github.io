---
layout: page
title: About me
permalink: /
---

{% include image.html url="/images/westheide.jpg" caption="Dr. Christian Westheide" width=300 align="right" %}

<p>I am a Senior Lecturer in Finance at the <a href="https://www.business-school.ed.ac.uk/" target="_blank">University of Edinburgh Business School</a>. I am also a Research Affiliate of the <a href="https://safe-frankfurt.de" target="_blank">Leibniz Institute for Financial Research SAFE</a>. My primary research focus is empirical financial market microstructure, with particular emphasis on European equity markets. In other research, I explore the interactions between institutional investors and firms and banks. Additionally, I contribute to meta-science studies.</p>
<br/>

<h2>News</h2>
<div class="news" >
<ul>
{% for item in site.data.news %}
<li>
<div class="newsdate"><b>{{item.date}}</b></div>  {{item.text}}
{% if item.post %}
<a href="/home/news/">more</a>
{% endif %}
</li>
{% endfor %}
</ul>

</div>
