# SMSAlert API Docs (Redoc + GitHub Pages)

This repository contains the **enterprise-ready** OpenAPI spec and a static Redoc site for **SMSAlert API v2.0.0**.

## Live docs
After enabling GitHub Pages (GitHub Actions), your docs will be available at:

`https://<your-org-or-user>.github.io/<repo-name>/`

## Auth
SMSAlert uses **HTTP Basic Auth** where:

- **username** = your SMSAlert username
- **password** = your API key

Example header:

```
Authorization: Basic base64(username:apiKey)
```

## Development
Open `index.html` locally (or serve with any static server). Redoc loads `openapi.yaml`.

## Deploy
This repo includes a GitHub Actions workflow that:
1) lints `openapi.yaml`
2) deploys the static site to GitHub Pages

## Files
- `openapi.yaml` – OpenAPI 3.1 spec (source of truth)
- `index.html` – Redoc entrypoint
- `.github/workflows/deploy.yml` – Pages deploy

