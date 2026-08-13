# Maverick — personal site

Single-page personal site (growth · marketing · web3 · AI). Interactive ASCII
portrait, scroll-driven hero collapse, and a contact form.

## Stack
Static site — no build step. Everything lives in `index.html` (inline CSS + JS),
with `avatar.png` as the portrait source. Third-party bits load over HTTPS at
runtime: Google Fonts, Lenis (smooth scroll, via unpkg), and FormSubmit for the
contact form.

## Run locally
Any static server, e.g.:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000

## Deploy
It's fully static, so any static host works (Vercel, Netlify, GitHub Pages,
Cloudflare Pages). `index.html` is the entry point at the repo root — no config
needed.

## Contact form
The form posts to [FormSubmit](https://formsubmit.co). The **first** submission
triggers a one-time activation email to the destination address; click the link
once and every later submission is delivered automatically.
