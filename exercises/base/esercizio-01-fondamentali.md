---
layout: default
title: "Esercizio Base 01: Fondamentali"
---

# Esercizio 01 — Fondamentali (Role + Task + Format)

## Scenario
Vuoi usare una chatbot per preparare una mail di follow-up dopo un colloquio conoscitivo (15 minuti) con un potenziale cliente.

## Obiettivo
Scrivere un prompt che produca una mail pronta da inviare, **professionale** e **breve**.

## Vincoli
- La mail deve essere in italiano.
- Deve includere: ringraziamento, 2 bullet con punti emersi, una proposta di prossimo step, chiusura.
- Non deve inventare dettagli non presenti.
- Se mancano informazioni, deve fare **max 3 domande** prima di scrivere la mail.

## Cosa consegnare
1) Il tuo prompt (in Markdown con sezioni).  
2) Una mini-checklist (3–5 punti) per valutare se l’output è buono.

## Rubric (0–2 ciascuno)
- Completezza (0–2): include tutti i blocchi richiesti.
- Specificità (0–2): vincoli chiari, poche ambiguità.
- Controllo formato (0–2): struttura dell’output imposta bene.
- Robustezza (0–2): gestione “manca info” + no inventare.

## Soluzione proposta (esempio)
```md
Ruolo: Sei un assistente commerciale (sales assistant) esperto in email B2B concise.

Contesto:
- Ho fatto un colloquio conoscitivo di 15 minuti con [NOME] di [AZIENDA].
- Note (inserisci qui): [INCOLLA NOTE]

Task:
1) Se nelle note mancano: obiettivo del cliente, prossimi step, o timing, fammi fino a 3 domande.
2) Altrimenti scrivi una mail di follow-up.

Vincoli:
- Non inventare dettagli oltre le note.
- Tono: professionale, diretto, non “salesy”.

Output (Format):
- Oggetto (1 riga)
- Corpo:
  - 1 frase di ringraziamento
  - 2 bullet: punti emersi (solo da note)
  - 1 frase: proposta prossimo step + 2 opzioni di slot (se non ho dati, chiedi)
  - Chiusura
```

## Errori comuni
- “Scrivi una mail di follow-up” senza note e senza regole → output generico.
- Nessun vincolo “non inventare” → dettagli allucinati.
- Nessuna gestione “manca info” → la mail esce comunque ma è sbagliata.
