---
layout: page
tagline: Tutorials at Interface of CS and Maths
---

# Tutorials

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | prepend: site.baseurl }}) 17:00 on {{ post.date | date: "%b %-d, %Y" }} at {{ post.venue }} {{ post.tagline }}
{% endfor %}

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>





