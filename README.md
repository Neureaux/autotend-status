# AutoTend Status

This repository contains the [Upptime](https://upptime.js.org) status page for AutoTend services.

Live status page: https://status.dev.autotend.io

## Monitored Services

| Service | URL |
|---------|-----|
| AutoTend App | https://app.dev.autotend.io |
| Marketing Site | https://dev.autotend.io |
| Admin Dashboard | https://admin.dev.autotend.io |
| Control Plane API | https://cp.dev.autotend.io |
| Deployment Dashboard | https://deploy.dev.autotend.io |

## Setup

1. Create a GitHub Personal Access Token (PAT) with `repo` and `workflow` scopes
2. Add it as a repository secret named `GH_PAT`
3. Enable GitHub Pages (Settings > Pages > Source: GitHub Actions)
4. Add CNAME record for `status.dev.autotend.io` pointing to `neureaux.github.io`

## How it works

- GitHub Actions checks all services every 5 minutes
- Results are stored in this repository
- A static status page is generated and deployed to GitHub Pages
- Incidents are automatically created when services go down
