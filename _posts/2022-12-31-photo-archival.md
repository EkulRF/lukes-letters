---
layout: post
title: Photography Archival Project (from the Summer of '22)
subtitle: Preserving old family photos, one scan at a time.
# gh-repo: daattali/beautiful-jekyll
# gh-badge: []
tags: [archival, photography]
comments: true
author: Luke RF
---

{% for post in paginator.posts %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.excerpt }}</p>
{% endfor %}

<div class="pagination">
  {% if paginator.previous_page %}
    <a href="{{ paginator.previous_page_path }}" class="previous">Previous</a>
  {% endif %}
  <span class="page-number">Page {{ paginator.page }} of {{ paginator.total_pages }}</span>
  {% if paginator.next_page %}
    <a href="{{ paginator.next_page_path }}" class="next">Next</a>
  {% endif %}
</div>

<a href="https://ekulrf.github.io/lukes-letters/photo-mum/">
  <img alt="Mum's Photos" src="https://lh3.googleusercontent.com/pw/ADCreHdmFjQIxu1AdI8vVeBnlWHq0Y8iPUksPQjpF7K0QgHXoJ-OMYsjYXChN4o_5FXwRwnHoJ_JTcvodpZmthezgDxhAXYbk1ON0i7NJd7M3CtB9rDQWtr4CPaRWJo-uc4y22gOEn2B4e3D6_5F4rZJ4r76=w1413-h955-s-no?authuser=1">
</a>

<a href="https://ekulrf.github.io/lukes-letters/photo-nan/">
  <img alt="Mum's Photos" src="https://lh3.googleusercontent.com/pw/ADCreHdGBpgwIIukrmqhCL0BipfO6RNbDSuEnrtSx5mYrgxXv8xrcQoF2pdXpp0sPAmvys9E0Uw6yNAEp8BTc-hQBYF4t9itL9VK_KtnVr-1VDK9Da4GErPPvYVErdQTH3Sq5znsrA63JZuBbqtV0X9Qi5lC=w1245-h955-s-no?authuser=1">
</a>
