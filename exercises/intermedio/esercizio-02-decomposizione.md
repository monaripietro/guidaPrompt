---
layout: default
title: "Esercizio Intermedio 02: Decomposition"
---

# Esercizio 02 — Decomposition (task complesso)

## Scenario
Devi scrivere una pagina di onboarding per un nuovo collega che entra nel team.

## Obiettivo
Scrivere un prompt che faccia:
1) scomposizione in sotto-sezioni,
2) bozza per sezione,
3) ricomposizione finale in un documento unico.

## Vincoli
- Output finale in Markdown con:
  - `## Chi siamo`
  - `## Cosa farai nelle prime 2 settimane`
  - `## Regole operative`
  - `## Dove trovare le informazioni`
  - `## FAQ`
- Chiedere 3 domande iniziali se mancano: ruolo, stack, priorità del team.

## Cosa consegnare
Il tuo prompt.

## Soluzione proposta (esempio)
```md
Ruolo: Sei un technical writer.

Prima di scrivere, fai 3 domande se mancano:
1) ruolo del nuovo collega
2) stack/strumenti principali
3) priorità del team nelle prossime 2 settimane

Poi:
Step A) Proponi un outline con le sezioni richieste + 2 bullet per sezione.
Step B) Scrivi una bozza per ogni sezione (max 120 parole).
Step C) Ricomponi in un singolo documento Markdown con i titoli richiesti.

Output: restituisci solo il documento finale (niente commenti extra).
```

## Errori comuni
- Outline e bozza mischiati senza fasi → aumenta confusione e ripetizioni.
