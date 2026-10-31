# STATUS

## What Was Built

A free, printable vehicle maintenance kit — 4 core tools, each delivered as both a Markdown file (editable in any text editor) and a styled, print-ready HTML file (open in browser → Print → PDF or paper). No accounts, no sign-ups, no data collection.

| File | Purpose |
|------|---------|
| `service-log.md` / `service-log.html` | Log routine services (oil changes, tire rotations, fluid flushes, filter replacements, belts, battery, alignment, etc.) with cost, next-due tracking, and 20 fillable rows (8 pre-filled examples + 12 blank) |
| `repair-tracker.md` / `repair-tracker.html` | Track unexpected repairs: symptoms, diagnosis, parts, labor cost, total cost, shop, warranty status, invoice numbers, and 20 fillable rows + symptom reference guide |
| `fuel-mileage.md` / `fuel-mileage.html` | Log fill-ups with odometer, gallons/liters, price/unit, total cost, trip miles, calculated MPG/km/L, cost per mile, and a 12-month summary table. 50 fillable rows |
| `maintenance-schedule.md` / `maintenance-schedule.html` | Manufacturer-recommended service intervals (20 items) with checkboxes, last-done/next-due dates, plus a custom-items table and a 4-season checklist |

Supporting files:
- `LICENSE` — MIT License with copyright line `Copyright (c) 2026 Asdale Dynamics, LLC`
- `README.md` — Overview, quick-start guide, print tips, vehicle info template, credits to Asdale Dynamics, LLC
- `STATUS.md` — This file

## How to Run It

This is a static, offline toolkit — no build step, no server, no dependencies.

**To fill digitally:**
- Open any `.md` file in a Markdown editor (Obsidian, VS Code, Typora, etc.) and type directly
- Edit the Markdown source to add/remove rows or change intervals

**To print:**
- Open any `.html` file in a web browser
- Press `Ctrl+P` (Windows/Linux) or `Cmd+P` (Mac)
- Select "Save as PDF" or print to paper
- For best results: enable "Print background graphics", set margins to "Minimum" or "None"

## Verification Results

- **Files present:** 11 files (4 .md, 4 .html, LICENSE, README.md, STATUS.md)
- **LICENSE copyright line:** Exactly `Copyright (c) 2026 Asdale Dynamics, LLC` — verified
- **README credit:** "Asdale Dynamics, LLC" appears 3 times — verified
- **HTML tag balance:** All 4 HTML files have balanced `<tr>`, `</tr>`, `<td>`, `</td>` tags — verified
- **HTML structure:** All 4 HTML files have proper `<!DOCTYPE html>` declaration and closing `</html>` — verified
- **No secrets/personal data:** Searched for API keys, passwords, tokens, secrets across all files — none found
- **No `.github/workflows` directory:** Confirmed absent
- **Git:** Repository initialized on `master`, all files committed (latest: `98d571d` + new commits) with plain commit messages (no Co-authored-by trailers)
- **Git identity:** Committed as existing identity (Dylan Asdale) — no co-author trailers
- **Typo fix:** "Wi per blades" → "Wiper blades" in maintenance-schedule.html (lines 110, 118) — fixed
- **README improved:** Added feature list, customization tips, clearer quick-start, file row counts

## Known Gaps

- **No dynamic calculation:** The HTML files are static print templates. MPG, cost/mile, and total cost must be calculated manually (formulas are documented in the Markdown and HTML pages).
- **No data persistence:** Nothing is saved between sessions. Markdown files are edited locally; HTML files are printed to PDF for permanent records.
- **No unit conversion:** The fuel-mileage page supports both US (gallons/MPG) and metric (liters/km/L) columns, but does not auto-convert between them.
- **No vehicle-specific defaults:** All intervals are "typical" ranges. The user must consult their owner's manual for exact specifications.
- **No digital export:** No CSV/JSON export, no app, no sync. This is intentionally a paper/print toolkit.
- **No browser compatibility testing:** HTML was validated for tag balance and structure, but rendering was not tested across all browser/print engine combinations.
- **TH closing tags optional:** HTML5 permits omitting `</th>`; all thead cells render correctly in browsers. Strict XML validation would flag this but it is valid HTML5.