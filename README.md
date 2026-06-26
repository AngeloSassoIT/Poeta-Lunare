# Poeta Lunare — Website

Sito statico per [Poeta Lunare](https://apps.apple.com/), il taccuino quotidiano sulla Luna per iOS.

Pensato per essere ospitato su GitHub Pages, servito su https://poetalunare.app.

## Struttura

| File | Scopo |
|---|---|
| `index.html` | Homepage con hero, funzionalità e CTA di download |
| `privacy.html` | Privacy policy (obbligatoria per App Store) |
| `support.html` | Pagina supporto con FAQ (obbligatoria per App Store) |
| `terms.html` | Termini d'uso |
| `404.html` | Pagina "non trovato" custom (servita da GitHub Pages su URL mancanti) |
| `style.css` | Foglio di stile condiviso (tema dark "cielo notturno") |
| `CNAME` | Dominio personalizzato per GitHub Pages (`poetalunare.app`) |
| `robots.txt` | Istruzioni per i crawler |
| `sitemap.xml` | Sitemap per i motori di ricerca |

## Anteprima locale

```bash
cd Files2
python3 -m http.server 8000
```

Poi apri http://localhost:8000

## Deploy

1. Push sul branch `main` del repo GitHub.
2. Repo Settings → Pages → Source: `main` / `/ (root)`.
3. Imposta il dominio personalizzato `poetalunare.app` e attiva **Enforce HTTPS**.

## Configurazione DNS (dominio personalizzato)

Dal tuo registrar (Cloudflare, Porkbun, ecc.) per `poetalunare.app`:

| Tipo | Nome | Valore |
|---|---|---|
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |
| CNAME | `www` | `<your-github-username>.github.io` |

Attendi 5-15 minuti per la propagazione DNS, poi attiva HTTPS nelle impostazioni del repo.

## Palette e identità

- Sfondo: navy notte profonda (`#050519`)
- Card: indaco (`#15193D`)
- Accent: oro chiaro / luna piena (`#e8c785`)
- Argento luna (`#b8c5d6`)
- Rosso luna di sangue (`#c97a64`)

Coerente con il tema dell'app iOS (`Theme.nightSky` in `Theme.swift`).

## Crediti

Le immagini lunari mostrate nel sito (favicon, hero) provengono dal patrimonio
NASA / JPL / USGS (missione Galileo, composito PIA00405) e sono di pubblico dominio.

## Licenza

© 2026 Angelo Sasso. Tutti i diritti riservati.
