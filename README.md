# SAGEA Tool

App PWA con strumenti per la sperimentazione agronomica in campo.
Struttura piatta: tutti i file vanno caricati allo stesso livello del repository, senza cartelle.

## File
- index.html — home
- schemi-blocchi.html — Schemi a Blocchi
- manifest.webmanifest, sw.js — installazione PWA e offline
- icon-192.png, icon-512.png, icon-maskable-512.png — icone

## Pubblicazione su GitHub Pages
1. Carica TUTTI i file nella radice del repository.
2. Settings → Pages → Deploy from a branch → main, / (root) → Save.
3. Dopo 1-2 minuti: https://TUONOME.github.io/NOME-REPO/

## Aggiornamenti
Quando carichi nuove versioni, incrementa CACHE in sw.js (sagea-v2 → sagea-v3, ...).
