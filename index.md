---
title: Home
layout: home
type: parent
order: 1
---

<div class="section header">
	<div class="container">
		<img src="{{ "/assets/img/logo.svg" | relative_url }}">
		<h3 class="section-heading">photography</h3>
		<p class="section-description">
			discovering the world with my vision
		</p>
		<div id="navbar-wrapper">
			<div id="navbar">
				<img id="brand" class="hide" src="{{ "/assets/img/logo.svg" | relative_url }}">
				{% assign mypages = site.pages | where: "type", "parent" | sort: "order" %}
				{% for page in mypages %}
				<a class="button" href="{{ page.url | relative_url }}">{{ page.title }}</a>
				{% endfor %}
			</div>
		</div>
	</div>
</div>

<div class="section main">
	<div class="container">
		<div class="row" id="gallery">
			<div class="column">
				<article class="thumb">
					<!-- <img class="lozad u-max-full-width" data-src="{{ coll.label | append: '/' | append: image.name }}" alt="{{ image.basename }}" /> -->
					<iframe width="960" height="540" src="https://www.youtube.com/embed/Dic2QqrEtUk" title="The Science of Coffee" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
				</article>
			</div>
			<!--<div class="one-half column">
				{% for image in list offset: l %}
				<article class="thumb">
					<img class="lozad u-max-full-width" data-src="{{ coll.label | append: '/' | append: image.name }}" alt="{{ image.basename }}" />
				</article>
				{% endfor %}
			</div>-->
		</div>
	</div>
</div>