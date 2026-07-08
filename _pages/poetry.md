---
layout: page
title: Poetry
permalink: /poetry/
nav: true
nav_order: 5
description: Original poetry collections.
---


> 「诗以载道，词以言情。」

欢迎来到我的诗词作品集。

---

{% assign poems = site.poetry | sort: "date" | reverse %}

{% for poem in poems %}

## [{{ poem.title }}]({{ poem.url | relative_url }})

> {{ poem.description }}

**创作时间：**

{{ poem.date | date: "%Y-%m-%d" }}

**分类：**

{{ poem.category }}

---

{% endfor %}