---
layout: page
title: Frequently Asked Questions
excerpt: "Questions that everyone asks."
search_omit: true
---

<ul class="post-list">
{% for faq in site.categories.faq %} 
  <li><article><a href="{{ site.url }}{{ faq.url }}">{{ faq.title }} <span class="entry-date"><time datetime="{{ faq.date | date_to_xmlschema }}">{{ faq.date | date: "%B %d, %Y" }}</time></span>{% if faq.excerpt %} <span class="excerpt">{{ faq.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
