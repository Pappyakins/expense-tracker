# Expense Tracker

A standalone, mobile-first expense tracking web app. Single `index.html` file —
inline CSS + vanilla JS, **zero external dependencies**. Works offline from
`file://` or any static host (including GitHub Pages). No build step.

## Features

- **Quick-add expenses** — amount, category, note, date (defaults to today); tap any entry to edit or delete. Validates amounts and blocks future dates.
- **Categories** — seeded set (Food, Transport, Shopping, Bills, Health, Entertainment, Groceries, Other) with icons; add/delete custom categories.
- **Dashboard** — month total header, today / this week / daily-average stats, spending-by-category donut chart, recent expenses, due-recurring suggestion chips.
- **Insights** — 30-day spending bar chart, top category, biggest single expense, this-week vs last-week comparison.
- **Budgets** — optional per-category monthly limits with progress bars and over/near-limit alerts.
- **Recurring expenses** — define weekly/monthly subscriptions; one-tap chips log them when due.
- **Search & filters** — by note text, category, and date range.
- **CSV export**, currency setting (default CAD), full data reset.
- **Privacy** — all data persists in `localStorage` on the device only.

## Hosting

Upload `index.html` anywhere static, or enable GitHub Pages on the repo
(Settings → Pages → Deploy from branch → `main` / `/`).

## Notes

- Data lives in `localStorage` under key `expenseTracker.v1` — per browser/device, no sync.
- Pure analytics helpers are exposed as `window.ET` for testing.
