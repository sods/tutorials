---
layout: page
tagline: Tutorials at Interface of CS and Maths
---

# Tutorials

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | prepend: site.baseurl }}) {% if post.time %} {{ post.time }} {% endif %} on {{ post.date | date: "%b %-d, %Y" }}{% if post.venue %} at **{{ post.venue }}**{% endif %}.{% if post.tagline %}*{{ post.tagline }}*.{% endif %}
{% endfor %}

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>





