---
layout: default
title: "Esercizio Avanzato 01: Self-consistency"
---

# Esercizio 01 — Self-consistency (3 soluzioni + scelta)

## Scenario
Devi scrivere una risposta a un cliente arrabbiato (mail breve) perché “il prodotto non funziona”.

## Obiettivo
Scrivere un prompt che generi 3 bozze indipendenti (A/B/C), le valuti con criteri, e poi restituisca **solo** la migliore.

## Vincoli
- Tono: calmo, empatico, professionale.
- Non promettere rimborsi o policy non citate.
- Output finale max 120 parole.

## Cosa consegnare
Il tuo prompt.

## Rubric (0–2 ciascuno)
- Indipendenza: A/B/C davvero diverse.
- Criteri: chiari e adatti (empatia, chiarezza, next step).
- Controllo: restituisce solo la migliore.

## Soluzione proposta (esempio)
```md
Ruolo: customer support lead.

Task:
1) Scrivi 3 bozze indipendenti (A/B/C).
2) Valuta ciascuna (0-2) su: Empatia, Chiarezza, Next step, Rischio promesse.
3) Scegli la bozza con punteggio più alto e riscrivila migliorata.

Vincoli:
- Max 120 parole.
- Non inventare policy (rimborsi, SLA, ecc.).

Output: restituisci solo la versione finale.
```
