# CampusSpend

CampusSpend is a private, browser-based expense tracker designed for student life in India. It helps students record income and expenses, set monthly spending limits, and understand how their money moves.

## Features

- Monthly overview of income, expenses, net cash flow, and budget remaining
- Add, edit, delete, search, filter, and sort transactions
- Per-category and overall monthly budgets with warning and overspend states
- Cash-flow, category, weekly, and month-over-month insights based on recorded data
- JSON backup and restore, plus transaction CSV export
- First-run sample data that can be cleared at any time
- Responsive desktop and mobile layouts; INR formatting

## Run locally on a Mac

No package installation or build step is needed. Open `index.html` in a browser, or run a small local server from this folder:

```sh
python3 -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000). Use a local server for the most reliable browser storage and file handling.

## Data and privacy

Transactions and budgets are stored in this browser's `localStorage` on the current device. They are not uploaded or synchronized. Use **Settings → Export JSON backup** to save a restorable copy, or export a CSV for spreadsheet use. Import validates the complete file before replacing existing data.

## Project structure

- `index.html` — application shell and accessible navigation
- `css/style.css` — responsive visual system and components
- `js/app.js` — local data model, calculations, rendering, charts, and interactions

## Screenshots

Screenshots can be added here after capturing the app at desktop and mobile sizes.

## Known limitations

- Data belongs to one browser profile and is not synchronized across devices.
- Category names are built in; custom categories are not currently supported.
- Charts are lightweight visual summaries rather than financial forecasting tools.

## Future ideas

- Optional custom categories and recurring transactions
- Installable offline app support
- Accessible downloadable charts and additional comparison periods
