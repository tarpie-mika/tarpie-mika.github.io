---
layout: layout.html
title: Posts Archive
altTitle: Posts Archive
youarehere:                  ^ you are here
---
	
<html lang="en">
	<head>
		<style>
			table {
				width: 0px;
				padding-left: 0px;
			}
			
			td {
				width: 50%;
			}
		</style>
	</head>
	<body>
		<br>
		<div class="boxInvis">
			<h1><u>Here you can read all my posts:</u></h1>
        </div>
        <div class="boxPink" style="padding-bottom: 5px; padding-top: 5px;">
			{% for post in collections.post %}
			<h3 style="margin-top: -0px;">✧ <a href="{{ post.url }}">{{ post.data.date | date: '%b %d, %Y', 'UCT' }}: {{ post.data.title }}</a></h3>
			<p style="margin-top: -20px;">&nbsp;&nbsp;&nbsp;&nbsp;{{ post.data.description }}</p>
			{% endfor %}
		</div>
	</body>
</html>