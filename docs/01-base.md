---
layout: default
title: Livello Base
---

# Livello Base — Fondamenti del prompt efficace

Obiettivo: passare da “scrivo una domanda” a “scrivo un’istruzione completa e verificabile”.

## 1) La formula minima (Role + Task + Format)

Un prompt robusto contiene quasi sempre:
- **Ruolo (Role)**: “Chi sei” (esperto, tutor, editor, analista…).
- **Compito (Task)**: cosa devi fare, con criteri di successo.
- **Formato (Format)**: come deve essere strutturato l’output.

Esempio (Markdown):
```md
Sei un tutor di matematica.
Task: spiega la differenza tra media e mediana a uno studente di 14 anni.
Format: 1) definizioni 2) esempio numerico 3) 3 errori comuni.
Tono: chiaro, incoraggiante, senza gergo.
```

## 2) Componenti di un prompt “completo”

Quando il problema è reale (non banale), aggiungi:

1. **Contesto (Context)**: informazioni necessarie, dati, testo da analizzare.
2. **Vincoli (Constraints)**: limiti (lunghezza, stile, ciò che non va fatto).
3. **Regole (Rules)**: priorità e comportamenti (es. “se manca info, fai domande”).
4. **Esempi (Examples)**: uno o due esempi di input/output desiderato.
5. **Criteri di qualità (Quality bar)**: come misurare “buono” (checklist o rubric).

Suggerimento: usa **delimitatori (delimiters)** per separare sezioni, così riduci ambiguità.

## 3) Delimitare e strutturare: Markdown e XML

### A) Markdown (consigliato per uso umano)
Pro:
- leggibile;
- facile separare sezioni con heading e code fence.

Template: vedi `templates/markdown-template.md`.

### B) XML (consigliato per “contratti” più rigidi)
Pro:
- sezioni esplicite;
- utile quando vuoi un output/struttura molto controllata.

Template: vedi `templates/xml-template.xml`.

## 4) Regole utili (Tips & Tricks)

- **Chiedi domande quando serve**: “Se mancano dati, fai fino a 3 domande prima di rispondere.”
- **Dichiara assunzioni**: “Se devi assumere, elenca assunzioni e procedi.”
- **Forza il formato**: “Rispondi solo con …” (lista, tabella, XML).
- **Riduci i gradi di libertà**: specifica audience, tono, lunghezza, esempi.
- **Separazione input/istruzioni**: metti sempre il testo da analizzare in una sezione dedicata.

## 5) Errori tipici (e fix rapidi)

- Troppo vago → aggiungi output format + criteri di successo.
- Mancano dati → aggiungi contesto o fai domande.
- Output incoerente → aggiungi delimitatori + schema fisso.
- Risposta “creativa” quando vuoi precisione → specifica “no inventare; se non sai, dillo”.

## Esercizi (Base)

Vai a `exercises/base/README.md`.
