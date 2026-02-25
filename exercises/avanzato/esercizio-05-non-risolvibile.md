---
layout: default
title: "Esercizio Avanzato 05: Non risolvibile"
---

# Esercizio 05 — Quando non è risolvibile (con un prompt)

## Scenario
Chiedi alla chatbot: “Fammi l’analisi completa dei competitor e dimmi chi sta crescendo di più.”
Non fornisci nomi dei competitor, né dati, né accesso al web.

## Obiettivo
Scrivere un prompt che **non finga** di poter completare il task, ma che:
1) spieghi cosa manca,
2) faccia domande mirate (max 3),
3) proponga un’alternativa utile “offline” (framework + template).

## Vincoli
- Output in Markdown con:
  - `## Cosa manca`
  - `## Domande`
  - `## Cosa posso fare subito (senza web)`
- Non inventare numeri o trend.

## Cosa consegnare
Il tuo prompt.

## Soluzione proposta (esempio)
```md
Ruolo: analista di mercato.

Task:
- Se non hai dati o accesso a fonti aggiornate, non inventare.
- Prima: spiega cosa manca per rispondere in modo “reale”.
- Poi: fai max 3 domande per ottenere input minimo.
- Infine: proponi un metodo utilizzabile subito senza web (framework + tabella da compilare).

Output (Markdown):
## Cosa manca
## Domande
## Cosa posso fare subito (senza web)
```

## Errori comuni
- “Sii creativo” → genera finti dati.
- Nessuna alternativa praticabile → l’utente resta bloccato.
