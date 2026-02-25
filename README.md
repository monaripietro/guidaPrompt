# Prompt Engineering Guide (3 livelli)

Guida pratica al prompt engineering, con teoria + esercizi svolti, divisa in:
**Base**, **Intermedio**, **Avanzato**.

Focus: prompt **testuali** (no tool-calling), con esempi strutturati in **Markdown** e **XML**.

## Come usare la guida

1. Parti da `docs/00-indice.md`.
2. Per ogni livello: leggi il modulo, poi svolgi gli esercizi della cartella `exercises/<livello>/`.
3. Quando un prompt “non funziona”, usa `docs/05-debugging-checklist.md` per migliorarlo in modo sistematico.
4. Se sei bloccato su “che tecnica uso?”, apri `docs/07-mappa-problema-tecnica.md`.

## GitHub Pages (sito)

Questo repository include i file minimi per pubblicare un sito con Jekyll via GitHub Pages.

- GitHub: `Settings → Pages → Build and deployment → Deploy from a branch`
- Branch: `main`
- Folder: `/(root)`
  
Nota: i link/CSS funzionano anche su GitHub Pages “project” (`https://<user>.github.io/<repo>/`) senza dover impostare `baseurl` manualmente.

## Struttura repository

- `docs/` — moduli didattici (base/intermedio/avanzato) + guida a LLM/LRM + checklist
- `templates/` — template pronti (Markdown/XML) da copiare e adattare
- `exercises/` — esercizi con: traccia, rubric (valutazione), soluzione proposta, errori comuni

## Obiettivo (risultati attesi)

Alla fine del livello avanzato dovresti saper:
- costruire prompt che risolvono problemi reali (con vincoli, formati e qualità misurabile);
- diagnosticare cosa è debole in un prompt (input, istruzioni, formato, vincoli, ambiguità, ecc.);
- capire quando **non** è ragionevole aspettarsi una soluzione solo via prompting/chatting.

## Licenza

MIT — vedi `LICENSE`.
