---
layout: default
title: "Esercizio Intermedio 05: Negative prompting"
---

# Esercizio 05 — Negative prompting (anti-goal chiari)

## Scenario
Stai scrivendo una descrizione prodotto (max 120 parole) per una pagina e-commerce.

## Obiettivo
Scrivere un prompt che riduca il rischio di:
- claim non verificabili,
- tono troppo “hype”,
- dettagli inventati.

## Vincoli
- Output in Markdown con:
  - `## Titolo` (max 8 parole)
  - `## Descrizione` (max 120 parole)
  - `## Specifiche` (3–5 bullet)
- Se mancano specifiche, chiedi max 3 domande prima di scrivere.

## Cosa consegnare
Il tuo prompt.

## Soluzione proposta (esempio)
```md
Ruolo: copywriter e-commerce (tono sobrio).

Regole:
- Se mancano informazioni chiave (materiali, dimensioni, compatibilità), fai max 3 domande.

Vincoli (Negative prompting):
- Non inventare specifiche o certificazioni.
- Non usare superlativi assoluti ("il migliore", "perfetto") senza dati.
- Non promettere risultati non verificabili.
- Evita slang e punti esclamativi.

Output (Markdown):
## Titolo
## Descrizione
## Specifiche
- ...
```

## Errori comuni
- Mettere solo divieti senza format → esce prosa disordinata.
- Non dire cosa fare se mancano dati → il modello “riempie i buchi”.
