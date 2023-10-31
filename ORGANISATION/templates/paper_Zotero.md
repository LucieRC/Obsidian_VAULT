---
tags: 
doi: "{{DOI}}"
citekey: "{{citekey}}"
read: 
authors: "{{authors}}"
date: '{{date.format("YYYY")}}'
aliases:
  - "{{shortTitle}}"
  - "{{citekey}}"
  - "{{title}}"
read_for: "{{ collections[0].name }}"
sub_read_for: "{% if collections[1] %}\r{{ collections[1].name}}{% else %}\r\r{% endif %}"
type: 
main_lab:
---

> [!Cite]
> {{bibliography}}

> [!PDF]
> {{pdfLink}}

{% persist "notes" %}
{% if isFirstImport %}
# 1. Introduction

# 2. Methods

# 3. Results

# 4. Discussion

# 5. Conclusion
{% endif %}
{% endpersist %}

