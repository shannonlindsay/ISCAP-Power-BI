---
title: Online Instructions
permalink: index.html
layout: home
---

Hyperlinks to everything you need to know about today's session are listed below. If you have any questions, you can submit a [GitHub issue](https://github.com/shannonlindsay/ISCAP-Power-BI/issues/new) or reach out to me via email.

## Power BI Links - labs and additional resources

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/Labs'" %}
| Topic | Link |
| --- | --- | 
{% for activity in labs  %}| {{ activity.lab.module }} | [{{ activity.lab.title }}{% if activity.lab.type %} - {{ activity.lab.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}
