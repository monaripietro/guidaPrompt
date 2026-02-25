---
layout: default
title: "Esercizio Avanzato 04: Refine"
---

# Esercizio 04 — Plan → Draft → Critique → Refine

## Scenario
Devi scrivere un messaggio (chat interna) per allineare un team su una decisione: cambiare priorità di una feature e posticiparla.

## Obiettivo
Scrivere un prompt che produca:
1) una bozza,
2) una critica guidata da checklist,
3) una versione finale migliorata.

## Vincoli
- Tono: fermo ma rispettoso.
- Deve includere: decisione, motivazione, impatto, next step.
- Output finale max 140 parole.
- Restituisci **solo** la versione finale (non includere bozza e critica).

## Cosa consegnare
Il tuo prompt.

## Soluzione proposta (esempio)
```md
Task: scrivi un messaggio di allineamento interno (max 140 parole).

Procedura:
Step 1) Draft: scrivi una bozza.
Step 2) Critique: valuta la bozza con checklist e segnala 3 miglioramenti.
Checklist:
- La decisione è chiara in 1 frase?
- La motivazione è concreta (non vaga)?
- Impatto e next step sono espliciti?
- Tono rispettoso e non accusatorio?
Step 3) Refine: riscrivi incorporando i miglioramenti.

Output: restituisci SOLO la versione finale.
```

## Errori comuni
- Chiedere bozza+critica+finale ma poi non imporre “solo finale” → output troppo lungo.
