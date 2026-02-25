---
layout: default
title: "Esercizio Intermedio 01: Few-shot"
---

# Esercizio 01 — Few-shot prompting (classificazione)

## Scenario
Stai moderando feedback utenti. Vuoi etichettare ogni messaggio come:
- `BUG`
- `FEATURE_REQUEST`
- `PRAISE`
- `OTHER`

## Obiettivo
Scrivere un prompt few-shot che:
- includa 4–6 esempi bilanciati;
- imponga un output in Markdown con tabella.

## Vincoli
- Una riga di tabella per messaggio: `id | label | reason (max 10 parole)`.
- Se ambiguo, label `OTHER`.

## Cosa consegnare
Il tuo prompt + i tuoi esempi.

## Rubric (0–2 ciascuno)
- Copertura esempi: esempi rappresentativi e non ridondanti.
- Controllo output: tabella rispettata.
- Regola ambiguità: `OTHER` usato correttamente.

## Soluzione proposta (esempio)
```md
Task: Classifica i messaggi.
Label set: BUG, FEATURE_REQUEST, PRAISE, OTHER.

Esempi:
- Input: "Dopo l'ultimo update crasha all'apertura" -> BUG
- Input: "Sarebbe utile esportare in PDF" -> FEATURE_REQUEST
- Input: "Interfaccia bellissima, bravi" -> PRAISE
- Input: "Come cambio la password?" -> OTHER

Output (Markdown table):
| id | label | reason |
|---:|---|---|

Messaggi:
1) ...
2) ...
```

## Errori comuni
- Esempi troppo simili → il modello overfitta a un caso.
- “reason” troppo lunga → aggiungi limite parole.
