---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<style type="text/css">
#dates { color: #808080; font-size: small; }
</style>
{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

<!---{% include base_path %}[comment:] --->

{% for post in site.publications reversed %}
  <b><a href="{{ post.url | prepend: site.resource }}.html"> {{ post.title }} </a></b>  
  <span id="dates">{{ post.date | date: "%B, %Y in " }} {{ post.venue }}</span>  
  {{ post.authornames | truncatewords: 6, " et al.," }}  
{% endfor %}


