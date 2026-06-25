# advisors.chat

> A board of advisors for every big decision.

The marketing site for **advisors.chat** — a decision-making studio where you bring
a hard call to a panel of minds you trust. They debate it in rounds (positions →
rebuttals → final vote) and hand you a verdict, the dissent, and the reasoning.
The workflow is defined in plain Markdown and run as a series of LLM calls; the
flagship example is `/boardroom`.

This repo is the **landing page** — a single static page, no build step.

## Stack

Plain HTML / CSS / vanilla JS. No framework, no bundler.

- `index.html` — the page
- `styles.css` — warm editorial light theme (Fraunces + Hanken Grotesk + JetBrains Mono)
- `script.js` — scroll reveals + nav state (progressive enhancement)
- `favicon.svg`

## Local preview

Any static server works:

```bash
python3 -m http.server 8000
# → http://localhost:8000
```

## Deploy (Vercel)

It's a static site, so no config is required.

```bash
vercel        # preview
vercel --prod # production
```

The custom domain `advisors.chat` is managed at the registrar (Porkbun) and
pointed at the Vercel deployment.
