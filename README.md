# Epstein Files — AI Newsroom (Netlify, DB‑frei)

## Netlify Settings
- Build command: `npm run build`
- Publish directory: `site`
- Functions directory: `netlify/functions`

## ENV (minimal)
Für volle Funktion:
- `GEMINI_API_KEY`
- `STRIPE_SECRET_KEY`
- `STRIPE_PRICE_ID_MONTHLY`
Optional:
- `GEMINI_MODEL` (default: gemini-1.5-flash)
- `SITE_URL` (fallback für success/cancel URLs)

Ohne Keys deployt die Seite trotzdem:
- ohne Gemini: Demo‑Modus (nur Quellen)
- ohne Stripe: Checkout zeigt Konfig‑Fehler

## Local
```bash
npm i
npm run build
npx netlify dev
```
