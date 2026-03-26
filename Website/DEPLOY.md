# Hosting

This folder is a static site. No build step is required.

## Files

- `index.html` — default entry point
- `world_cup_master_analytics_2010_2022.json` — dashboard data
- `team_player_spotlights_2026.json` — player spotlight data

## Fastest options

### GitHub Pages

1. Create a new GitHub repo.
2. Upload the contents of the `Website/` folder to the repo root.
3. In GitHub:
   `Settings -> Pages -> Build and deployment -> Deploy from a branch`
4. Select:
   `Branch: main`
   `Folder: / (root)`
5. Open the published Pages URL.

### Netlify

1. Drag the `Website/` folder into Netlify Drop.
2. Netlify will publish it immediately.

### Vercel

1. Import the project into Vercel.
2. Set the project root to `Website/`.
3. Framework preset:
   `Other`
4. No build command is needed.

## Local test

From the project root:

```bash
cd Website
python3 -m http.server 8000
```

Then open:

`http://localhost:8000`

## Important note

The dashboard uses `fetch()` for local JSON files, so it must be served through a web server or a static host.
