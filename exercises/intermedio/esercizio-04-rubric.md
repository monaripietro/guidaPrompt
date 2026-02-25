---
layout: default
title: "Esercizio Intermedio 04: Rubric"
---

# Esercizio 04 — Rubric prompting (qualità misurabile)

## Scenario
Vuoi una spiegazione breve (max 180 parole) di un concetto a scelta (es. “overfitting”, “cache”, “inflazione”) per un pubblico beginner.

## Obiettivo
Scrivere un prompt che:
1) chieda una prima versione,
2) la valuti con una rubric,
3) la migliori una sola volta se necessario.

## Vincoli
- Output finale in Markdown con:
  - `## Spiegazione`
  - `## Esempio`
  - `## Errori comuni` (3 bullet)
- Vietato usare gergo non spiegato.

## Cosa consegnare
Il tuo prompt (in Markdown).

## Rubric (0–2 ciascuno)
- Chiarezza: linguaggio semplice, concetti definiti.
- Accuratezza: niente semplificazioni fuorvianti.
- Completezza: include esempio + errori comuni.

## Soluzione proposta (esempio)
```md
Task: spiega [CONCETTO] a un principiante (max 180 parole).

Output (Markdown):
## Spiegazione
## Esempio
## Errori comuni
- ...

Qualità (Rubric 0–2):
- Chiarezza
- Accuratezza
- Completezza

Procedura:
1) Scrivi una prima versione.
2) Assegna i punteggi e spiega in 1 riga cosa manca se <2.
3) Se un punteggio è <2, riscrivi una sola volta e restituisci SOLO la versione finale.
```

## Errori comuni
- Chiedere “migliora finché perfetto” → loop e output lungo.
- Rubric vaga (“sii chiaro”) senza scala → autovalutazione inutile.
