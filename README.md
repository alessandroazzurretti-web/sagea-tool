# SAGEA Tool

App PWA con strumenti per la sperimentazione agronomica in campo.

## Struttura
- `index.html` — home con l'elenco degli strumenti
- `tools/schemi-blocchi.html` — Schemi a Blocchi (RCBD a serpentina)
- `manifest.webmanifest` — dati di installazione PWA
- `sw.js` — service worker (cache offline)
- `icons/` — icone dell'app

## Pubblicazione su GitHub Pages
1. Crea un repository (es. `sagea-tool`) e carica **tutti** i file mantenendo la struttura.
2. Nel repo: Settings → Pages → Source: "Deploy from a branch" → branch `main`, cartella `/ (root)` → Save.
3. Dopo qualche minuto l'app è su `https://TUONOME.github.io/sagea-tool/`.

## Installazione sul telefono
- **Android (Chrome)**: apri il link → banner o menu ⋮ → "Installa app".
- **iPhone (Safari)**: apri il link → tasto Condividi → "Aggiungi alla schermata Home".

Dopo la prima apertura online l'app funziona anche **senza connessione**.

## Aggiornamenti
Quando carichi nuove versioni dei file, incrementa `CACHE` in `sw.js`
(es. `sagea-v1` → `sagea-v2`) così i telefoni scaricano la versione nuova.

## Aggiungere un nuovo strumento
1. Crea `tools/nome-strumento.html`.
2. Aggiungi la card in `index.html`.
3. Aggiungi il percorso in `ASSETS` dentro `sw.js` e incrementa `CACHE`.
