# Receipt Vault — Ebbers Construction

A comprehensive receipt management system built for construction businesses. Upload PDF receipts, track spending, compare prices across vendors, and generate business reports.

## Features

- **AI-Powered PDF Parsing** — Upload receipt PDFs and Claude AI extracts store, date, PO numbers, line items, quantities, and prices automatically
- **Multi-Store Support** — Tracks purchases from Menards, Home Depot, Lowe's, Scheels, gas stations, and more
- **Pricing History** — Compare prices for the same material across stores and over time with interactive charts
- **Job Costing** — Group receipts by PO/job name to see total project costs with breakdowns
- **Business Reports** — Printable charts and graphs: spending trends, store breakdowns, category analysis
- **Search** — Find any item, SKU, store, or PO across all receipts instantly
- **Store Management** — Upload custom logos, add contact info, track per-vendor spending
- **Duplicate Detection** — Multi-layer dedup prevents the same receipt from being uploaded twice
- **Persistent Storage** — All data saves to localStorage and persists across sessions

## Setup

### GitHub Pages (Simplest)

1. Create a new GitHub repository
2. Upload `index.html` to the root of the repo
3. Go to **Settings → Pages → Source** and select "Deploy from a branch" → `main` → `/ (root)`
4. Your site will be live at `https://yourusername.github.io/repo-name/`

### Local

Just open `index.html` in a browser. No build step, no server needed.

### Custom Domain

1. Deploy to GitHub Pages as above
2. In **Settings → Pages → Custom domain**, enter your domain
3. Add a CNAME record pointing to `yourusername.github.io`

## Tech Stack

- React 18 (loaded from CDN)
- Babel (in-browser JSX compilation)
- Anthropic Claude API (for receipt parsing)
- SVG charts (no chart library dependencies)
- localStorage for persistence

## How It Works

1. **Upload** — Drop a PDF receipt on the Upload tab
2. **Parse** — Claude AI reads each page and extracts structured data
3. **Track** — Receipts appear in the system with full line item detail
4. **Analyze** — Use Pricing History, Jobs, Reports, and Search to understand your spending

## License

Private — Ebbers Construction LLC
