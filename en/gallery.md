---
title: Propaganda
layout: page
lang: en
---
<div class="row wrapper">
	{% for prop in site.data.props_list %}
        <a href="{{site.url}}{{site.baseurl}}/public/propaganda/{{prop[1]["name"]}}">
		<img src="{{site.url}}{{site.baseurl}}/public/propaganda/{{prop[1]["name"]}}" alt="{{site.url}}{{site.baseurl}}/public/propaganda/{{prop[1]["description"]}}" width="400" ></a>
	{% endfor %}
</div>

