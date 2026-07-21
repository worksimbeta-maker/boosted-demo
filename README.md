# Boosted · Pannello demo

Showcase online delle demo Boosted. È la versione web del "raccoglitore" che gira in locale
con `Avvia Boosted.command`, riscritta per funzionare come sito statico su GitHub Pages.

## Cosa contiene

| Scheda | Contenuto | Tipo |
|---|---|---|
| **▶ Come funziona** | `presentazione-boosted.html` — presentazione animata dei sistemi | statica |
| **Ecommerce** | vetrina, operatori, scanner, titolare, marketing | live (Vercel) |
| **Ordini al tavolo · QR** | prenotazioni, sala, cucina KDS, cameriere, titolare, assistente | live (Vercel) + presentazione |
| **Parrucchiere · Salone** | `demo-parrucchiere.html` — prenotazioni, prova look AI, agenda, gestionale | statica |
| **Materiali** | assistente chiamate, listino enoteca | statiche |

Le schede **Ecommerce** e **Ordini QR** sono app Node/Express con stato su file: non girano su
GitHub Pages (solo statico). I loro URL live (deploy su Vercel) si impostano nella variabile
`LIVE` in cima a [`index.html`](index.html); finché sono vuoti, la scheda mostra la presentazione
o un messaggio "in arrivo".

## In locale

Basta un qualsiasi server statico nella cartella, es.:

```
npx serve .
```

## Nota

Nessuna chiave o credenziale è inclusa in questo repo (vedi `.gitignore`).
