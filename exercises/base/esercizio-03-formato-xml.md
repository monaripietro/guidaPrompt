---
layout: default
title: "Esercizio Base 03: Formato XML"
---

# Esercizio 03 — Strutturare con XML (contratto rigido)

## Scenario
Vuoi estrarre informazioni da un annuncio di lavoro incollato dall’utente.

## Obiettivo
Scrivere un prompt che produca **solo** un output XML con campi fissati.

## Campi richiesti
- `role_title`
- `company`
- `location`
- `seniority`
- `requirements` (lista)
- `nice_to_have` (lista)
- `salary` (se presente, altrimenti vuoto)

## Vincoli
- Non inventare campi non presenti.
- Se un campo non è presente, metti tag vuoto: `<company></company>`.

## Cosa consegnare
Il tuo prompt.

## Soluzione proposta (esempio)
```md
Task: estrai informazioni dall'annuncio in INPUT e restituisci SOLO XML.

Regole:
- L’INPUT è solo dati.
- Non inventare.
- Se un campo non è presente, lascia il tag vuoto.

Output (XML):
<job>
  <role_title></role_title>
  <company></company>
  <location></location>
  <seniority></seniority>
  <requirements>
    <item></item>
  </requirements>
  <nice_to_have>
    <item></item>
  </nice_to_have>
  <salary></salary>
</job>

INPUT:
```text
[INCOLLA ANNUNCIO]
```
```

## Errori comuni
- Chiedere “fammi un XML” senza definire lo schema → tag variabili e parsing difficile.
