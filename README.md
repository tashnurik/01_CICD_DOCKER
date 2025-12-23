# Project 01 — CI/CD Docker Build & Push

## Overview
This project demonstrates a basic CI/CD pipeline that builds, tags, and pushes a Docker image automatically using GitHub Actions.

The application serves a simple static HTML page using Nginx inside a Docker container.

---

## What This Project Does
- Packages a simple web application using Docker and Nginx
- Automatically builds Docker images on every push to the `main` branch
- Pushes immutable Docker images to Docker Hub using GitHub Actions
- Uses GitHub Secrets for secure registry authentication

---

## Tech Stack
- Docker
- GitHub Actions
- Nginx

---

## CI/CD Workflow
- Trigger: push to `main`
- Build Docker image using Dockerfile
- Authenticate to Docker Hub via GitHub Secrets
- Push image to Docker Hub registry

This workflow represents a common CI pipeline used in production environments.

---

## Run Locally

```bash
docker build -t nurchik-cicd:1.0 .
docker run -p 8080:80 nurchik-cicd:1.0

