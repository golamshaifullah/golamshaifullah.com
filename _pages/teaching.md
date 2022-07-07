---
layout: archive
title: "Teaching"
permalink: /teaching/
author_profile: true
---

<style type="text/css">
 #dates { color: #808080; font-size: small; }
</style>

{% include base_path %}

{% for post in site.teaching reversed %}
  <b><a href="{{ post.url | prepend: site.resource }}.html"> {{ post.title }} </a></b>  
  <span id="dates">{{ post.period }}</span>  
  {{ post.venue }}  
{% endfor %}
