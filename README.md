# Sito di Poeta Lunare (GitHub Pages)

Sito statico dell'app **Poeta Lunare** — nessun build step, solo HTML/CSS.

## Contenuto

- `index.html` — landing page (funzioni, screenshot, supporto)
- `privacy.html` — informativa privacy (da usare anche come Privacy Policy URL in App Store Connect)
- `assets/` — icona app, favicon e screenshot
- `.nojekyll` — disattiva Jekyll su GitHub Pages

## Pubblicazione su GitHub Pages (branch `main`)

1. Crea un repository su GitHub (es. `poeta-lunare`).
2. Copia **il contenuto di questa cartella** nella root del repository e fai push su `main`:
   ```bash
   cd website
   git init
   git add .
   git commit -m "Sito Poeta Lunare"
   git branch -M main
   git remote add origin https://github.com/<tuo-utente>/poeta-lunare.git
   git push -u origin main
   ```
3. Su GitHub: **Settings → Pages → Build and deployment**
   - Source: *Deploy from a branch*
   - Branch: `main` / cartella `/ (root)`
4. Il sito sarà disponibile su `https://<tuo-utente>.github.io/poeta-lunare/`.

## Da fare dopo la pubblicazione dell'app

- In `index.html`, sostituisci `href="#"` del bottone **App Store** con il link reale dell'app.
- Usa l'URL del sito come **Support URL** e `privacy.html` come **Privacy Policy URL** in App Store Connect.
