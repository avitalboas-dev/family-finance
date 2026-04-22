# Family Finance

A lightweight, single-page finance tracker for Revolut CSV exports. No accounts, no backend — runs entirely in your browser.

**Live app → [avitalboas-dev.github.io/family-finance](https://avitalboas-dev.github.io/family-finance/)**

---

## How it works

1. Export a CSV from the Revolut app (Documents & Statements → CSV)
2. Drop the file onto the upload screen
3. Browse your spending by category, view monthly flow, and search or filter transactions

Data never leaves your device. The only thing stored remotely is the category mapping file in this repo.

---

## Features

- **Spending & income breakdown** by category, with click-through to filter transactions
- **Monthly flow chart** showing income vs. spending over time
- **Period selector** — current month (default), last 3 months, last 6 months, all time, or a custom date range
- **Sortable transactions table** — click any column header to sort by date, description, category, or amount
- **Category editor** — reassign any transaction's category; changes apply across all matching merchants and persist across sessions
- **Export categories** — download `revolut-categories.json` to commit back to the repo and share across devices

---

## Category persistence

Category edits are saved to your browser's `localStorage` and auto-loaded from `revolut-categories.json` in this repo on each visit.

To sync edits across browsers or devices:
1. Click **↓ Export & save categories** in the transactions panel
2. Replace `revolut-categories.json` in this repo with the downloaded file
3. Commit and push — all browsers will pick up the new categories on next load

---

## Local development

No build step needed. Just open `index.html` in a browser.

```bash
# Serve locally (avoids fetch restrictions on file:// URLs)
npx serve .
```

---

## Deployment

The app is deployed via GitHub Pages from the `main` branch root. Any push to `main` updates the live site within a minute or two.
