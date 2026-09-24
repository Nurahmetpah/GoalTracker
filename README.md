# Goal Tracker

A single-file personal goal tracker (`index.html`) for a one-year plan (Oct 2026 – Sep 2027) across four directions: Mandarin, System Analysis, YouTube (hard cap), and Coursework.

## Use it

Open `index.html` in a browser. No build or server needed. To use it on your phone, host it anywhere static (e.g. enable GitHub Pages for this repo) and "Add to Home Screen".

Data lives in `localStorage` under the key `goaltracker:v1` — **per browser, per device**. Use **Settings → Export JSON** regularly; the dashboard nags you after 14 days without a backup.

## Features

- **Logging** — one-tap `+15 / +30 / +60` per direction, or the `+` button (keyboard: `L`) for custom minutes, notes and past dates. Every log has Undo. Edit/delete from **History**.
- **Streaks** — a day counts at ≥ the minimum viable session (default 10 min, configurable). "Never miss twice": one missed day shows a warning, two in a row resets. Current + best streak, 14-day strip.
- **Weekly progress** — targets with a pace marker; YouTube shown against its cap (amber near, red over).
- **If-then & obstacle plans**, grouped by direction on the dashboard.
- **Milestones** with countdowns; seeded titles have no dates — set them.
- **Statistics** — per-direction 12-week charts, 6-month heatmaps, averages, % of weeks target hit / under cap, side-by-side comparison, and share of time.
- **Weekly review** — prompted on Sundays (and if last week's was skipped); saves a snapshot + your notes; last week's "what I'll change" is shown back to you all week.

Charts use Chart.js from jsDelivr; everything else works offline, with a table fallback for charts.
