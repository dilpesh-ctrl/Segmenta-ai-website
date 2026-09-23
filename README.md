# Segmenta AI — marketing website

Single-page marketing site for [segmenta-ai.com](https://segmenta-ai.com).
Bid floor optimisation for mobile apps and games, without an SDK.

## Structure

| Path | What it is |
|---|---|
| `index.html` | The entire site. Self-contained: inline CSS and JS, no build step, no dependencies. |
| `docs/website-copy.md` | Source copy and positioning notes. |
| `docs/privacy-content.md` | Draft privacy policy and form micro-copy. Needs legal review. |

## Running it

Open `index.html` in a browser. There is nothing to install.

## Deploying

The site is a single static file, so any static host works. For GitHub Pages:
Settings → Pages → Source: `main` branch, `/ (root)`.

## Before launch

- [ ] **Wire up the Join form.** The submit handler logs to the browser console and sends nothing. See the `TODO` block at the bottom of `index.html`.
- [ ] **Self-host the How It Works diagram.** It is currently hot-linked to a CloudFront URL that may expire. Download it into `assets/` and update the `src`.
- [ ] **Add a privacy policy page** and link it from the Join form.
- [ ] **Add spam protection** to the form (honeypot field or captcha).
- [ ] **Verify the team section figures** — the combined revenue claim and job titles.
- [ ] Replace `hello@segmenta-ai.com` if that is not the right address.

## Fonts

Archivo, Instrument Sans and JetBrains Mono, loaded from Google Fonts.
