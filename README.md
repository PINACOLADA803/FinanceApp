[README.md](https://github.com/user-attachments/files/31107457/README.md)
# Finance — Personal Finance Tracker

A self-contained personal finance dashboard that runs entirely in the browser — no backend, no build step, no dependencies to install. Track income and expenses, manage budgets, monitor recurring costs and debts, and back up your data — all from a single HTML file.

**[Live demo](https://PINACOLADA803.github.io/FinanceApp/)** — replace with your actual GitHub Pages URL once enabled.

## Features

- **Dashboard** — total balance, income, expenses, and savings rate, with a selectable date range (this month, last month, custom, etc.)
- **Transactions** — add, edit, delete income and expenses; filter by type, category, date range, or search
- **Categories** — fully customizable income/expense categories with colors and icons; renaming or deleting a category updates existing transactions automatically
- **Budgets** — set a monthly budget per expense category, with color-coded progress bars (green/orange/red)
- **Recurring costs** — mark any transaction as daily, weekly, monthly, or yearly; future occurrences are generated automatically without duplicates
- **Debts** — track loans, credit cards, and other debts, with payoff progress, interest rate, minimum payment, and due date
- **Charts** — income vs. expenses over time, expense breakdown by category, and monthly cash flow (via Chart.js)
- **Reports** — top spending categories, highest expense, and monthly averages over a selected period
- **Currency display** — switch between EUR, USD, GBP, CHF, SEK, NOK, and DKK (display only, no conversion)
- **Dark / light mode** — toggle and persisted across sessions
- **Export / Import** — download your data as JSON (full backup) or CSV (transactions), and restore from a JSON backup
- **Automatic backups** — optional daily backup download, plus a reminder banner if it's been a while since your last one
- **Mobile-ready** — responsive layout, iOS safe-area support, and "Add to Home Screen" support for a full-screen app feel on iPhone

## Getting started

No installation required.

1. Open `index.html` directly in any modern browser, **or**
2. Visit the [hosted version](https://PINACOLADA803.github.io/FinanceApp/) if GitHub Pages is enabled for this repo.

Your data is stored in your browser's `localStorage`, tied to that specific browser and origin. It is **not** synced across devices or shared between users — each person who opens the app gets their own independent, empty tracker.

### Backing up your data

Because everything is stored locally in the browser, it's a good idea to back up regularly:

- **Settings → Export as JSON** — full backup of transactions, categories, budgets, debts, and settings
- **Settings → Export transactions as CSV** — spreadsheet-friendly transaction list
- **Settings → Automatic backups** — toggle a daily automatic JSON download
- **Settings → Import** — restore from a previously exported JSON backup

## Running locally

Since this is a single static HTML file, you can simply download and open it:

```bash
git clone https://github.com/PINACOLADA803/FinanceApp.git
cd FinanceApp
open index.html   # macOS
# or double-click index.html in your file explorer
```

## Hosting on GitHub Pages

1. Push `index.html` to the `main` branch of this repository (at the root, not in a subfolder).
2. Go to **Settings → Pages**.
3. Under "Build and deployment," set **Source** to "Deploy from a branch," choose branch `main` and folder `/ (root)`, then save.
4. Your app will be live at `https://<your-username>.github.io/<repo-name>/` within a couple of minutes.

## Tech stack

- HTML5, CSS3, vanilla JavaScript — no framework, no build tools
- [Chart.js](https://www.chartjs.org/) (loaded via CDN) for charts
- Browser `localStorage` for persistence

## License

Add a license of your choice (e.g. MIT) if you plan to share or open-source this project.
