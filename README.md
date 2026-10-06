# Investment Portfolios Tracker

Static tracker for 3 Wealthsimple portfolios (Conservative, High Growth, Growth Core).

## How it works

- **Holdings, cost basis and trades** live in `index.html` — the `const P` array in the `<script>` block plus the per-portfolio Activity tables.
- **Prices** are a static snapshot stored in `let live`. Snapshot date (from the page's status bar): **Oct 6, 2026 (~11:39am ET, intraday)**.
- The **Refresh** button only works inside the old Cowork artifact runtime. Anywhere else it falls back to the snapshot above.
- **No API keys or secrets** are used. Open `index.html` directly in a browser — there is no build step.
