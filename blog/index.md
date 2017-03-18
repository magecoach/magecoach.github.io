---
layout: default
title: The mage.coach blog
description: The latest news from the mage.coach world
keywords: mage.coach, ray bogman, ronald bethlehem
nav: blog
---

# Blog


{% for post in site.posts %}

<a href="{{ site.baseurl }}{{ post.url }} title="{{ post.title }}">
<amp-img noloading width="100" height="100" alt="{{ post.title }}" layout="responsive" src="{{site.static-url}}{{ post.authorimage }}" class="photo pull-left"></amp-img></a>

## [{{ post.title }}]({{ site.baseurl }}{{ post.url }})

**{{ post.date | date: '%Y' }}-{{ post.date | date: '%m' }}-{{ post.date | date: '%d' }}** -
  {{ post.intro }}

  [>> Read more]({{site.baseurl}}{{ post.url }})



  * * *

{% endfor %}
