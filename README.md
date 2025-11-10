# 🐳 My Node Docker App

A simple **Node.js app** containerized with **Docker** and automated using **GitHub Actions CI/CD**.

## 🚀 Workflow
This pipeline:
1. Builds a Docker image
2. Tags it with the Git commit SHA
3. Pushes it to Docker Hub
4. Deploys and runs the latest image

## ⚙️ Local Run
```bash
docker build -t my-node-docker-app .
docker run -d -p 3000:3000 my-node-docker-app
