---
layout: default
title: "Esercizio Intermedio 03: CoT pratico"
---

# Esercizio 03 — CoT “pratico” (brief rationale + verifica)

## Scenario
Vuoi un piano di studio di 7 giorni per imparare un argomento (a scelta).

## Obiettivo
Scrivere un prompt che:
- chieda un piano giorno-per-giorno;
- chieda una breve spiegazione delle scelte (brief rationale);
- includa una checklist di verifica.

## Vincoli
- Piano in tabella Markdown: `Day | Goal | Activities | Output`.
- Brief rationale: max 5 bullet totali.
- Checklist finale: 5 item.

## Cosa consegnare
Il tuo prompt.

## Soluzione proposta (esempio)
```md
Task: crea un piano di studio di 7 giorni su [ARGOMENTO] per un principiante.

Output:
1) Tabella Markdown: Day | Goal | Activities | Output
2) Brief rationale (max 5 bullet): perché questa sequenza
3) Checklist (5 item): come verificare i progressi

Vincoli:
- Attività realistiche (max 60 min/giorno).
- Non dare link: descrivi attività auto-contenute.
```

## Errori comuni
- “Spiega passo passo il ragionamento” → output lungo e meno utile; meglio rationale breve + checklist.
