---
layout: default
title: Repository
---

{% include base.html %}

# Repository

## README (sito)

{% capture readme_md %}{% include_relative README.md %}{% endcapture %}
{{ readme_md | markdownify }}

## Contributing

- {% capture p %}{% link contribuire.md %}{% endcapture %}[Linee guida]({{ site_base }}{{ p }})

