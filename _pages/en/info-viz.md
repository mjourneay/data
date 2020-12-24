---
altLangPrefix: autre-page
dateModified: 2020-01-08
description: 
  en: Info Viz
footer: true
langtoggle: true
lang: en
noMainContainer: false
sitemenu: true
sitesearch: true
title: Another page
---

<h2>{{ page.description.en }}</h2>

<ul>
  {% for page in site.pages %}
  {% if page.path contains 'en/data' %}
    <li>
      <a href="{{ site.baseurl }}{{ page.url }}">{{ page.contentTitle.en }}</a>
    </li>
    {% endif %}
  {% endfor %}
</ul>
