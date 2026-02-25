---
layout: default
title: Debugging Checklist
---

# Debugging Checklist — Migliorare un prompt che non funziona

Usala quando l’output è: incompleto, vago, sbagliato, incoerente, troppo lungo, troppo creativo.

## 1) Input

- Ho dato tutti i dati necessari?
- Ho separato chiaramente **INPUT** (dati) e **INSTRUCTIONS** (compito)?
- Ho usato delimitatori (Markdown/XML)?

## 2) Istruzioni

- Il task è un verbo operativo? (es. “estrai”, “confronta”, “riscrivi”, “genera”)
- Ho definito criteri di successo verificabili?
- Ho indicato cosa fare se manca info? (domande / assunzioni)

## 3) Formato output

- È specificato lo schema? (headings, bullet, tabella, XML tags)
- Ho chiesto “solo output” (se serve) per evitare prosa inutile?

## 4) Vincoli e priorità

- Ho messo “non inventare” se serve?
- Ho specificato la priorità delle regole (se confliggono)?

## 5) Qualità

- Ho incluso una checklist/rubric di auto-controllo?
- Ho limitato le iterazioni di refine (max 1–2)?

## 6) Diagnosi finale (se ancora non va)

Chiediti: questo task richiede strumenti esterni, dati mancanti, o decisioni non specificate?
Se sì, cambia obiettivo: “chiedi info mancante + proponi opzioni”.
