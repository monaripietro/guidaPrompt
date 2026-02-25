---
layout: default
title: Licenza
---

{% capture license_txt %}{% include_relative LICENSE %}{% endcapture %}

# Licenza

```text
{{ license_txt | strip }}
```

