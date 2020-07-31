---
title: "Styles Directory"
layout: page
---

## All Styles

<ul class="features features__flexible">
{%- for style in collections.allStyles -%}
	<li>
		<span>
			<a href="/styles/{{ style.data.style.title | slug }}">{{ style.data.style.title }}<span aria-hidden="true"></span></a>
			<span>by {{ style.data.style.author}}</span>
		</span>
	</li>
{%- else -%}
	<li class="empty">
		<span>
			Awaiting your contribution!
		</span>
	</li>
{%- endfor -%}
</ul>
