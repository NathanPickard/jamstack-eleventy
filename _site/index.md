---
title: Welcome
date: Created
layout: base
tags:
  - home
  - welcome
  - info
---

# {{ title }}
**Date**: {{ page.date.toUTCString() }}

**By**: {{ pkg.author }}

This project is built with the JAMStack and eleventy

<ul>
  {% for item in tags %}
  <li>{{ item }}</li>
  {% endfor %}
</ul>