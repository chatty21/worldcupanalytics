# FIFA World Cup Viewership Analytics Dashboard

An interactive World Cup analytics dashboard exploring tournament audience trends from **2010 to 2022**, with a **2026 forecasting layer** built on team strength, popularity, recent form, and player-availability signals.

## Live Project

- Live demo: `Add your Vercel link here`
- GitHub repo: `https://github.com/chatty21/worldcupanalytics`

## Overview

This project was built as a sports analytics and data storytelling product rather than a static dashboard. It combines historical tournament-level and match-level analytics with interactive forecasting for the 2026 FIFA World Cup.

The dashboard includes:

- historical match-by-match audience analysis
- stage-wise viewership trends
- most-watched matches and teams
- top FIFA-ranked team analytics
- 2026 scenario forecasting
- broadcaster expectation modeling
- interactive match simulator
- player spotlight cards based on projected impact signals
- timeline and geographic storytelling sections

## Features

- **Historical analytics**
  Viewership, attendance, stage performance, and team-based insights across 2010, 2014, 2018, and 2022.

- **2026 forecasting**
  Match and tournament forecasts using modeled audience signals.

- **Interactive simulator**
  Users can choose teams, stage, host country, drama level, and availability assumptions to estimate projected audience.

- **Player spotlight module**
  Displays a featured player to watch for the selected teams using form, star-power, and availability assumptions.

- **Football-themed UI**
  A visual design inspired by live football broadcasts rather than a standard BI report.

## Tech Stack

- `HTML`
- `CSS`
- `JavaScript`
- `JSON`
- `Chart.js`
- `GitHub`
- `Vercel`

## Project Structure

```text
.
├── README.md
├── Data Files/
│   ├── world_cup_master_analytics_2010_2022.csv
│   ├── world_cup_dataset1_attendance_2010_2022.csv
│   ├── ...
├── Website/
│   ├── index.html
│   ├── worldcupanalytics_data_driven.html
│   ├── world_cup_master_analytics_2010_2022.json
│   ├── team_player_spotlights_2026.json
│   ├── vercel.json
│   └── DEPLOY.md
└── archives/
    └── worldcupanalytics.html
```

## Local Run

Because the dashboard uses `fetch()` to read JSON files, it must be served through a local web server.

From the repo root:

```bash
cd Website
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Deployment

This project is configured for static hosting on **Vercel**.

Recommended Vercel settings:

- Framework Preset: `Other`
- Root Directory: `Website`
- Build Command: empty
- Output Directory: empty

See [Website/DEPLOY.md](./Website/DEPLOY.md) for quick deployment notes.

## Notes

- Some 2026 values are **forecasted/model-based**, not official FIFA projections.
- Player spotlight imagery depends on external sources and fallbacks.
- The historical file used by the dashboard is a hybrid analytics layer intended for storytelling and forecasting, not a pure raw-observed archive.

## Author

**Chaitanya Patil**

- GitHub: `https://github.com/chatty21`
- LinkedIn: add your LinkedIn URL here

