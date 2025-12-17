# Project 01 — CI/CD Docker Build & Push

## What this project does
- Serves a simple HTML page using Nginx in Docker
- Uses GitHub Actions to build and push the Docker image to Docker Hub on every push to `main`

## Tech Stack
- Docker
- GitHub Actions
- Nginx

## Run locally
```bash
docker build -t nurchik-cicd:1.0 .
docker run -p 8080:80 nurchik-cicd:1.0

