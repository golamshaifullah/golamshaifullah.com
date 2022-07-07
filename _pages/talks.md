---
layout: archive
title: "Talks"
permalink: /talks/
author_profile: true
---

<style type="text/css">
 #dates { color: #808080; font-size: small; }
</style>

{% include base_path %}

{% for post in site.talks reversed %}
  <b><a href="{{ post.url | prepend: site.resource }}.html"> {{ post.title }} </a></b>  
  <span id="dates">{{ post.date | date: "%B %Y" }}</span>  
  {{ post.type }} at {{ post.venue }}  
{% endfor %}
