# Luap Chips Ltd: reports and videos

Management reports, dashboards and videos for **Luap Chips Ltd**, a fictitious UK distributor that buys computer chips in bulk and sells them in smaller packs to business customers.

The material is written for a board of directors, senior management team and lead investors, many of whom are not finance specialists. It was created to demonstrate AI-assisted financial reporting.

**[Open the site](https://ronnoc.org/reports/)**

> This is for demonstration purposes only; Luap Chips Ltd is a fictitious company and all data has been artificially generated.

## Contents

| Item | Type | Folder |
|---|---|---|
| Management results report | Interactive report | [`management-results/`](management-results/) |
| Investor profile | Interactive report | [`investor-profile/`](investor-profile/) |
| Results for the nine months to 30 September 2026: a message from the leadership team | Video, 3 min 2 s, 16:9 | [`leadership-message/`](leadership-message/) |
| Nine months in motion | Video, 1 min 10 s, 4:5 for social media | [`nine-months-in-motion/`](nine-months-in-motion/) |

The top-level `index.html` is the landing page that lists everything above.

### Management results report

The board, senior management and investor pack covering January 2024 to September 2026, with budgets for 2025 and 2026. A period selector switches between the nine months to 30 September 2026, the full year 2025 and the full year 2024.

| Tab | Contents |
|---|---|
| Key indicators | A headline summary and eight KPIs, each compared with the prior year and the budget |
| Commentary | Management commentary on performance against budget, trading, margin, costs, cash and working capital, and the areas of focus for the board |
| Against budget | Waterfall charts from budgeted to actual profit and cash, sales by product group against budget, and line-by-line profit and loss and balance sheet comparisons |
| Trading | Month-by-month results for each year against budget, and where each £1 of sales goes |
| Customers and products | Sales and margin by product group, customer sector and region, and the ten largest customers |
| Cash and funding | Cash and bank borrowing over time, cash received and paid, and the three bank covenant tests |
| Working capital | Debtor, stock and creditor days, debtor ageing, the largest overdue accounts, and stock by product group |
| Definitions | How each measure is defined and how the figures and budgets were prepared |

Features: interactive charts, PDF export of the whole report, a searchable help panel with a glossary of financial terms (no AI service or account needed), light and dark themes, and layouts for phones, tablets and desktops.

### Videos

- **Leadership message:** the managing director, finance director, sales director and operations director each present the highlights of the nine months. Captions are shown on screen.
- **Nine months in motion:** a short animated video made for LinkedIn, showing how chips move through the warehouse and the headline numbers for January to September 2026.

Each video has its own page with a player, a download link and the disclaimer.

## Folder layout

```
index.html                    landing page
README.md
management-results/
    index.html                the interactive report
    preview.jpg               thumbnail for the landing page
investor-profile/
    index.html                the investor profile report
    preview.jpg               thumbnail for the landing page
leadership-message/
    index.html                player page
    video.mp4
    poster.jpg                still shown before the video plays
nine-months-in-motion/
    index.html
    video.mp4
    poster.jpg
```

## Adding a new report or video

1. Create a folder with a short, lower-case name, such as `cash-forecast/`.
2. Put the report in it as `index.html`; for a video, add `video.mp4`, `poster.jpg` and a player page copied from one of the existing video folders.
3. Add a card for it to the landing page (`index.html`) and a row to the table above.

Keep each video under 25 MB so it can be uploaded through the GitHub website.

## How it was built

The figures were derived from three source workbooks: an artificially generated ledger (trial balance, sales invoices, cash book, debtor and creditor listings and stock valuation) and the 2025 and 2026 budgets. They were reconciled to the trial balance and embedded in the report. The report, pages and videos were produced with Claude, Anthropic's AI assistant.

## Technical notes

- Every page is a self-contained HTML file. There is no server or database.
- The report loads the [jsPDF](https://github.com/parallax/jsPDF) library from cdnjs for its PDF export; all pages load fonts from Google Fonts.
- Videos are H.264 MP4 files that play in the browser's built-in player.

## Disclaimer

This is for demonstration purposes only; Luap Chips Ltd is a fictitious company and all data has been artificially generated. The people shown in the videos are fictitious and their images were generated by AI. Any resemblance to real companies or people is coincidental.
