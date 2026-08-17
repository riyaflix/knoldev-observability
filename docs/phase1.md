# Phase 1: Platform Foundation

## What was built
- Local Kubernetes cluster using Kind
- Sample FastAPI application (`/`, `/health` endpoints)
- Dockerized application
- Helm chart for deployment
- CI/CD pipeline via GitHub Actions: build → lint → deploy → smoke test

## Key components
| Component | Tool |
|---|---|
| Container Platform | Docker |
| Kubernetes | Kind |
| Package Manager | Helm |
| CI/CD | GitHub Actions |

## Pipeline stages
1. Build Docker image
2. Lint Helm chart
3. Create Kind cluster
4. Load image into cluster
5. Deploy with Helm
6. Smoke test (`/health` check)
