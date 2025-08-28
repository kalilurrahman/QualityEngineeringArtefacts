---
layout: page
title: Strategy & Approach PDFs
permalink: /strategy-list/
---

# Strategy & Approach Content

Below is a list of our strategy and approach PDF resources:

<ul>
  {% assign pdfs = site.static_files | where_exp: "file", "file.path contains '/' and file.extname == '.pdf'" %}
  {% for pdf in pdfs %}
    <li>
      <a href="{{ pdf.path | relative_url }}" target="_blank">{{ pdf.name }}</a>
    </li>
  {% endfor %}
</ul>
