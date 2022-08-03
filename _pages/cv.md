---
layout: page
permalink: /cv/
title: CV
description: Within this page you can view or download my CV. It will be updated periodically. For any inquiries or questions please do not hesitate to contact me.
nav: true
nav_order: 4
---
{% assign rootpath = '/' | relative_url %}
In case the inline PDF does not appear, you may download the PDF file [here]({{ example_pdf.pdf | prepend: pathprefix | relative_url }}).
{% pdf site.cv.pdf | page.title | rootpath %}
