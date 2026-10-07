# Ambulance MDT UK

A UK-style ambulance mobile data terminal (MDT) / CAD frontend designed for training, roleplay and simulation projects.

## Features

- Interactive Blackpool map
- Incident queue with C1-C4 priorities
- Incident creation and management
- Unit status controls
- Road routing / sat-nav
- Address and postcode search
- Turn-by-turn route information
- Patient and incident details
- Incident notes and history
- MDT/control messaging UI
- Responsive desktop/tablet layout
- Browser-side persistence for selected settings and notes

## Run locally

Open `index.html` in a modern browser.

For the most reliable behaviour, serve the folder through a small local HTTP server rather than opening the file directly. For example:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

## GitHub Pages

This repository includes a GitHub Actions workflow under `.github/workflows/deploy-pages.yml`.

After uploading the repository to GitHub:

1. Open **Settings → Pages**.
2. Set the source to **GitHub Actions** if GitHub has not already selected it.
3. Push changes to the `main` branch.
4. GitHub Actions will deploy the site to GitHub Pages.

## External services

The frontend uses third-party web services for mapping, geocoding and routing. Their availability, usage limits and terms can change. For a production deployment, use providers appropriate for your expected traffic and comply with their attribution and usage requirements.

## Important

This is a frontend prototype. It does **not** provide a secure multi-user CAD backend, authentication, database, real-time unit tracking, or real emergency-service dispatch integration.

Do not use it for real emergency-service operations or real patient data.
