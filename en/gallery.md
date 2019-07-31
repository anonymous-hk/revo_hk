---
title: Propaganda
layout: page
lang: en
---
All propaganda credits go to a large group of unnamed Hongkongers. If you would like to supoort us, please donate to the free press in Hong Kong instead of us:)

The table below shows a list of trustable press and charities:

|Press/Charities	|Link|
|---				|--- |
|612 Humanitarian Relief Fund|https://www.facebook.com/612Fund/|
|Hong Kong Free Press|https://www.hongkongfp.com/support-hkfp/|

<div class="row wrapper">
	{% for prop in site.data.props_list %}
        <a href="{{site.url}}{{site.baseurl}}/public/propaganda/{{prop[1]["name"]}}">
		<img src="{{site.url}}{{site.baseurl}}/public/propaganda/{{prop[1]["name"]}}" alt="{{site.url}}{{site.baseurl}}/public/propaganda/{{prop[1]["description"]}}" width="400" ></a>
	{% endfor %}
</div>

