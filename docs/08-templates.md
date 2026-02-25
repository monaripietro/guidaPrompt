---
layout: default
title: Template
---

{% include base.html %}

# Template pronti (Markdown/XML)

## Template Markdown

Usa questo come base quando vuoi un prompt leggibile e “copiabile”:

- {% capture p %}{% link templates/markdown-template.md %}{% endcapture %}[Template prompt (Markdown)]({{ site_base }}{{ p }})

## Template XML

Utile quando vuoi un “contratto” di sezioni molto rigido (soprattutto per estrazione).

- File XML (scaricabile): [`templates/xml-template.xml`]({{ site_base }}/templates/xml-template.xml)
