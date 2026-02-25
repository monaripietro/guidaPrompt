---
layout: default
title: Home
---

{% include base.html %}

# Prompt Engineering Guide

Guida pratica al prompt engineering, con teoria + esercizi, divisa in 3 livelli: **Base**, **Intermedio**, **Avanzato**.

## Inizia da qui

- {% capture p %}{% link docs/00-indice.md %}{% endcapture %}[Indice]({{ site_base }}{{ p }})
- {% capture p %}{% link docs/07-mappa-problema-tecnica.md %}{% endcapture %}[Mappa “problema → tecnica”]({{ site_base }}{{ p }})
- {% capture p %}{% link docs/05-debugging-checklist.md %}{% endcapture %}[Debugging checklist]({{ site_base }}{{ p }})

## Livelli

- {% capture p %}{% link docs/01-base.md %}{% endcapture %}[Livello Base]({{ site_base }}{{ p }})
- {% capture p %}{% link docs/02-intermedio.md %}{% endcapture %}[Livello Intermedio]({{ site_base }}{{ p }})
- {% capture p %}{% link docs/03-avanzato.md %}{% endcapture %}[Livello Avanzato]({{ site_base }}{{ p }})

## Esercizi

- {% capture p %}{% link exercises/base/README.md %}{% endcapture %}[Esercizi Base]({{ site_base }}{{ p }})
- {% capture p %}{% link exercises/intermedio/README.md %}{% endcapture %}[Esercizi Intermedio]({{ site_base }}{{ p }})
- {% capture p %}{% link exercises/avanzato/README.md %}{% endcapture %}[Esercizi Avanzato]({{ site_base }}{{ p }})
