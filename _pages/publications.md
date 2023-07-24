---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

You can find my articles on [Google Scholar](https://scholar.google.com/citations?user=K7Q4GWQAAAAJ&hl=zh-CN)

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
