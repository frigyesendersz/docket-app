# Docket

A to-do list with optional due dates, plus a calendar view for deadlines (with project tags), sorted by urgency.

## Running locally

It's a single static file — no build step. Open `index.html` directly, or serve it:

```bash
python3 -m http.server 4173
```

## Deploying

Deployed as a static site on Vercel. No framework, no build command — Vercel serves `index.html` as-is.

## Notes on data storage

This standalone version stores tasks in the browser's `localStorage`, so data is **per-browser**, not synced across devices. (A separate copy of this app lives as a Claude Artifact, which syncs across devices via Claude's shared storage — this GitHub/Vercel copy is the portable, framework-free version.)
