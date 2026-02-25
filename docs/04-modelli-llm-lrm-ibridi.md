---
layout: default
title: Modelli (LLM, LRM, Ibridi)
---

# Prompt per modelli con e senza reasoning (LLM, LRM, ibridi)

Obiettivo: adattare il prompt in base a **capacità di reasoning** e **budget** (tempo/token).

## Glossario minimo

- **LLM (Large Language Model)**: ottimo su linguaggio, stile, riassunti, classificazione; può “saltare” passaggi in task multi-step.
- **LRM (Large Reasoning Model)**: ottimizzato per ragionamento multi-step (pianificazione, logica, problemi più lunghi).
- **Ibridi**: modelli che possono operare in modalità “standard” o “reasoning/thinking” (a volte con parametri o modalità specifiche).

> Nota: i nomi commerciali cambiano spesso. Questa guida resta **vendor-neutral** e ti dà pattern che funzionano in generale.

## 1) Prompting per LLM senza reasoning “forte”

Obiettivo: ridurre “salti” e aumentare controllo.

Preferisci:
- istruzioni **sequenziali** e brevi;
- output con **schema** (Markdown/XML);
- esempi (few-shot) quando lo stile o la policy contano;
- “se manca info → fai domande”.

Pattern:
```md
Task: ...
Vincoli: ...
Format: ...
Procedura:
1) ...
2) ...
3) ...
Se non puoi completare, chiedi chiarimenti (max 3).
```

## 2) Prompting per LRM (reasoning nativo)

Obiettivo: sfruttare reasoning senza chiedere “rumore”.

Preferisci:
- obiettivo chiaro + criteri di successo;
- verifiche (checklist) e controlli finali;
- “brief rationale” (non un flusso lungo) quando serve trasparenza.

Pattern:
```md
Obiettivo: ...
Criteri di successo: ...
Output: ...
Prima di rispondere, verifica:
- copertura requisiti
- coerenza interna
- edge cases principali
Restituisci: output + 3 bullet di rationale (max).
```

## 3) Prompting per modelli ibridi (standard + reasoning)

Problema: lo stesso prompt può rendere **troppo lento** (reasoning sempre) o **troppo superficiale** (reasoning mai).

Pattern “compatibile” (degrada bene):
```md
Se il modello supporta una modalità di reasoning più profonda, usala per questo task.
Altrimenti, segui la procedura in passi e verifica con la checklist finale.
```

Consiglio pratico:
- aggiungi un **budget di profondità** (“massimo 2 iterazioni di refine”, “max 6 passi”);
- chiedi un **controllo finale** invece di “spiega tutto il ragionamento”.
- se il provider usa un **system prompt** per abilitare/ottimizzare il reasoning, evita di sovrascriverlo “a vuoto”: rischi di degradare la modalità (controlla la doc ufficiale del modello).

## 4) Indicazioni su chain-of-thought (CoT) nella pratica

- Se vuoi affidabilità: chiedi **struttura + verifiche**.
- Se vuoi trasparenza: chiedi una **spiegazione breve** (rationale) o di mostrare **solo** i passaggi necessari (es. calcoli).
- Evita di incentivare testo “di ragionamento” non necessario: aumenta lunghezza e a volte peggiora precisione.
