---
title: Welcome
date: Created
layout: page
tags:
  - home
  - welcome
  - info
---

# {{ title }}
**Date**: {{ page.date | simpleDate }}

**By**: {{ pkg.author }}

This project is built with the JAMStack and eleventy

<ul>
  {% for item in tags %}
  <li>{{ item | capitalize }}</li>
  {% endfor %}
</ul>