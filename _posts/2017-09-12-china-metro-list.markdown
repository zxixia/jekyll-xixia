---
layout: post
title:  "中国城市地铁信息汇总"
categories: Favorite
tags: Metro
author: 西夏
description: 中国所有已开通地铁的城市信息汇总。
---


<div style="width: 802px; background-color: rgb(204, 232, 207);">
	<div style="position:relative;width:800px;border:1px solid lightgray">
		<a title="中国已开通轨道交通城市一览">
			<img alt="中国已开通轨道交通城市一览" src="/assets/images/post/2017-09-12-china-metro-list/map/map.png" width="800" height="637" style="background-color: rgb(204, 232, 207);">
		</a>
		
		<!-- 后面紧跟的就是城市坐标 -->
		{% for metro in site.data.metro.maps %}
			<div style="position:absolute;top:{{ metro.top }};left:{{ metro.left }}">
				<div style="position:absolute;left:-4px;top:-4px;line-height:0">
					<b>
						<img alt="{{ metro.city }}" src="/assets/images/post/2017-09-12-china-metro-list/map/8px-Red_pog.svg.png" title="{{ metro.city }}">
					</b>
				</div>
				<div style="font-size:90%;line-height:110%;position:absolute;width:6em;
					{% if metro.text_top %}top:{{ metro.text_top }};{% endif %}
					{% if metro.text_bottom %}bottom:{{ metro.text_bottom }};{% endif %}
					{% if metro.text_left %}left:{{ metro.text_left }};{% endif %}
					{% if metro.text_right %}right:{{ metro.text_right }};{% endif %}
					text-align:left">
					<b>
						<span style="padding:1px">
							<a href="{{ metro.url }}" title="{{ metro.urlTitle }}">{{ metro.city }}</a>
						</span>
					</b>
				</div>
			</div>
		{% endfor %}

	</div>
</div>

---

<table border="1" class="text-center">
  <tr bgcolor="#eaecf0">
  	<th width="160px" class="text-center">标识</th>
    <th width="50px" class="text-center">序号</th>
    <th width="150px" class="text-center">开通时间</th>
    <th width="150px" class="text-center">城市</th>
    <th width="150px" class="text-center">运营线路数</th>
    <th width="150px" class="text-center">通车里程</th>
    <th width="200px" class="text-center">官方网站</th>
  </tr>
  
	{% for metro in site.data.metro.metros %}
		<tr height="80px">
	    <td bgcolor="#eaecf0">
	    	<img src="/assets/images/post/2017-09-12-china-metro-list/{{ metro.logo }}" {% if metro.imgWidth %} width="{{ metro.imgWidth }}" {% endif %}/>
	    </td>
	    <td>{{ forloop.index }}</td>
	    <td>{{ metro.year }}</td>
	    <td>{{ metro.city }}</td>
	    <td>{{ metro.line }}</td>
	    <td>{{ metro.miles }}公里</td>
	    <td><a href= "{{ metro.url }}">{{ metro.urlTitle }}</a></td>
	  </tr>
	{% endfor %}
    
</table>



<!-- 后面是文章参考资料 -->
<br/>
### 参考资料：

1，[维基百科-中国城市轨道交通系统][wiki-china-metro-list]

2，[地铁族-两岸四地城市轨道交通开通情况][ditiezu-pages]

3，[UrbanRail.net][urbanrail-net]

<!-- 文章插图和超链接 -->

[wiki-china-metro-list]: https://zh.wikipedia.org/wiki/%E4%B8%AD%E5%9B%BD%E5%9F%8E%E5%B8%82%E8%BD%A8%E9%81%93%E4%BA%A4%E9%80%9A%E7%B3%BB%E7%BB%9F
[ditiezu-pages]: http://www.ditiezu.com/thread-497320-1-1.html
[urbanrail-net]: http://www.urbanrail.net/
