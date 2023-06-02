---
title: IISER
layout: parent
description: I miss IISER sometimes
type: parent
order: 3
---

<div class="section main">
	<div class="container">
		{% assign mypages = site.pages | where: "type", page.title %}
		{% for page in mypages %}
		<a class="button" href="{{ page.url | relative_url }}">{{ page.title }}</a>
		{% endfor %}
	</div>
</div>