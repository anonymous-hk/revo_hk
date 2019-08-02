---
title: Propaganda
layout: page
lang: zh-hs
---

所有文宣工具由一群香港人所制作。如您想支持我们，请踊跃捐款至其他媒体或援助基金。

|媒体/援助基金	|网址|
|---				|--- |
|612人道支援基金612|<a href="https://www.facebook.com/612Fund/">https://www.facebook.com/612Fund/</a>|
|Hong Kong Free Press|<a href="https://www.hongkongfp.com/support-hkfp/">https://www.hongkongfp.com/support-hkfp/</a>|

<br>
<br>
<div class="row wrapper">
	{% for prop in site.data.props_list %}
        <a href="{{site.url}}{{site.baseurl}}/public/propaganda/{{prop[1]["name"]}}">
		<img src="{{site.url}}{{site.baseurl}}/public/propaganda/{{prop[1]["name"]}}" alt="{{site.url}}{{site.baseurl}}/public/propaganda/{{prop[1]["description"]}}" width="400" ></a>
	{% endfor %}
</div>