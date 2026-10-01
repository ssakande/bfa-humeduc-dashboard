# Burkina Faso Humanitarian Dashboard

Interactive geospatial dashboard for humanitarian and education data in Burkina Faso, built with React, React-Leaflet and Recharts.

## Local development

```bash
npm ci
npm start
```

The application opens at `http://localhost:3000`.

## Production build

```bash
npm run build
```

The production files are generated in the `build/` folder.

## Deploy to GitHub Pages

This repository is configured for:

`https://ssakande.github.io/burkina-dashboard/`

The GitHub Actions workflow automatically builds the application and publishes the `build/` folder to the `gh-pages` branch whenever changes are pushed to `main`.

In GitHub, go to **Settings → Pages** and select **Deploy from a branch**, then choose:

- Branch: `gh-pages`
- Folder: `/ (root)`

If the repository is configured to use **GitHub Actions** as the Pages source instead, use the workflow as the deployment mechanism and do not configure a second branch-based deployment.

## Manual deployment

If you prefer to deploy from your computer:

```bash
npm run deploy
```

This runs the production build first and then publishes `build/` to the `gh-pages` branch.
