---
layout: default
title: Livello Intermedio
---

# Livello Intermedio — Tecniche e strategie “nominabili”

Obiettivo: collegare **problema → tecnica → prompt pattern**.

## Prima regola: non è magia, è gestione dell’ambiguità

Molte tecniche servono a:
- ridurre ambiguità;
- aumentare copertura dei casi;
- rendere l’output verificabile.

## 1) Few-shot prompting

**Cos’è**: dai 2–5 esempi (input → output) per “mostrare” lo standard.

**Quando usarlo**:
- classificazione / estrazione;
- stile coerente;
- policy di risposta (“se X allora Y”).

**Pattern (mini)**:
```md
Task: etichetta ogni frase come {POS, NEG, NEU}.
Esempi:
- Input: "Ottimo servizio" -> Output: POS
- Input: "Non mi piace" -> Output: NEG
Ora etichetta:
1) ...
```

Esercizio: [Few-shot]({{ site_base }}/exercises/intermedio/esercizio-01-few-shot/).

## 2) Chain-of-Thought (CoT) / Step-by-step

**Idea**: spezzare un problema in passi logici.

**Uso pratico consigliato** (senza “chain-of-thought verboso”):
- chiedi **struttura e verifiche**, non un monologo di ragionamento;
- preferisci “**brief rationale**” o “passi ad alto livello” + risultato.

Pattern:
```md
Risolvi il problema.
Poi:
1) elenca i passi ad alto livello (max 6 bullet)
2) mostra i calcoli solo dove necessario
3) verifica con un controllo finale
```

Esercizio: [CoT rationale]({{ site_base }}/exercises/intermedio/esercizio-03-cot-rationale/).

## 3) Decomposition (scomposizione)

**Cos’è**: trasformare un task grande in sotto-task più piccoli.

**Quando**:
- requisiti complessi;
- output lungo;
- alta probabilità di dimenticanze.

Pattern:
```md
1) Fai una lista di sotto-task.
2) Esegui ogni sotto-task in ordine.
3) Ricomponi in un output finale unico.
```

Esercizio: [Decomposizione]({{ site_base }}/exercises/intermedio/esercizio-02-decomposizione/).

## 4) Rubric prompting (criteri di valutazione)

**Cos’è**: dai una rubric (0–2 / 0–5) e chiedi di auto-valutare l’output.

**Perché funziona**: rende “buono” misurabile e riduce risposte generiche.

Pattern:
```md
Scrivi la risposta.
Poi valuta con questa rubric:
- Accuratezza (0-2)
- Completezza (0-2)
- Chiarezza (0-2)
Se un punteggio è <2, migliora e ripeti una volta.
```

Esercizio: [Rubric]({{ site_base }}/exercises/intermedio/esercizio-04-rubric/).

## 5) Negative prompting (cosa NON fare)

**Cos’è**: elenco di divieti/anti-goal.

**Quando**:
- allucinazioni frequenti;
- tono/stile fuori target;
- output troppo lungo o troppo “fantasioso”.

Esempio:
```md
Vincoli:
- Non inventare dati o fonti.
- Non includere premesse non richieste.
- Se manca info, fai domande.
```

Esercizio: [Negative prompting]({{ site_base }}/exercises/intermedio/esercizio-05-negative-prompting/).

## Esercizi (Intermedio)

Vai a [Esercizi intermedio]({{ site_base }}/exercises/intermedio/).
