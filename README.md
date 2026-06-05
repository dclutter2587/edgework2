# EdgeWork — NHL DFS Analytics

Professional NHL Daily Fantasy projection tool built around 5v5, even strength, and all-strength analysis with penalty kill boosts.

## Deploy to Vercel (5 minutes)

1. Go to [vercel.com](https://vercel.com) and sign up / log in (free)
2. Click **Add New → Project**
3. Click **Upload** (bottom of the page)
4. Drag the `edgework` folder here and drop it
5. Click **Deploy**
6. Your live URL appears: `edgework.vercel.app` (or similar)

To use a custom domain like `edgework.com`:
- Buy the domain (~$12/yr) at Namecheap or Google Domains
- In Vercel: Settings → Domains → Add → follow the DNS instructions

## Update the site

Any time you want changes:
1. Make edits to `index.html` here with Claude
2. Re-upload the folder to Vercel (or connect GitHub for auto-deploy)
3. Same URL, updated instantly

## Features

- **Rankings tab** — sortable by any metric, filterable by strength type, team, position
- **Matchup tab** — line-by-line view with projections
- **Import tab** — DK salary CSV paste + NST Google Apps Script
- **Settings tab** — tune projection weights live

## NST Auto-Import (Google Apps Script)

1. Open your Google Sheet → Extensions → Apps Script
2. Paste the script from the Import tab (click "Copy Full Script")
3. Run `setDailyTrigger()` once
4. Data pulls every day at 8am automatically

## Data Sources

- DraftKings salary CSV (manual daily paste)
- Natural Stat Trick (via Apps Script server-side fetch)
- Manual overrides for injuries / line changes / goalie confirms
