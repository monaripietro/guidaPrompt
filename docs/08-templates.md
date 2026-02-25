---
layout: default
title: Template
---

# Template pronti (Markdown/XML)

## Template Markdown

Usa questo come base quando vuoi un prompt leggibile e “copiabile”:

- {% capture p %}{% link templates/markdown-template.md %}{% endcapture %}[Template prompt (Markdown)]({{ p | relative_url }})

## Template XML

Utile quando vuoi un “contratto” di sezioni molto rigido (soprattutto per estrazione).

- File XML (scaricabile): [`templates/xml-template.xml`]({{ '/templates/xml-template.xml' | relative_url }})

