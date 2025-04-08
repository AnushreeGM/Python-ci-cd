# CI/CD Pipeline with Docker, Kubernetes, and Jenkins

This project demonstrates a CI/CD pipeline that automates the build, containerization, and deployment of a Python web application using Docker, Kubernetes, and Jenkins.

---

## 🚀 Project Overview

The pipeline is designed to:

- Package and containerize the app
- Push the Docker image to DockerHub
- Deploy the image to a Kubernetes cluster
- Scale the deployment up and down
- Automate all steps via a Jenkins pipeline triggered by GitHub webhooks

---

## 📂 Tech Stack

- Python
- Docker
- Kubernetes (via Minikube or managed cluster)
- Jenkins (Declarative Pipeline)
- GitHub
- DockerHub

---

## 🔨 Tasks Performed

- Forked and cloned the sample Python application from GitHub.
- Packaged the application into a zip archive (excluding `.git` files).
- Wrote a `Dockerfile` to containerize the application.
- Built and pushed the Docker image to DockerHub:  
  👉 [`anushreegm12/python-app:latest`](https://hub.docker.com/r/anushreegm12/python-app)

- Created Kubernetes configuration files:
  - `deployment.yaml` to deploy the Docker image
  - `service.yaml` to expose the app via NodePort
- Deployed the application using `kubectl apply`
- Verified deployment and accessed service using `curl <NodeIP>:<NodePort>`

- Scaled the deployment to 3 replicas using:
  ```bash
  kubectl scale deployment python-app --replicas=3

 - Scaled the deployment to 1 replicas using:
  ```bash
  kubectl scale deployment python-app --replicas=1

---
🔗 Useful Links
GitHub Repo: https://github.com/anushreegm/python-ci-cd

DockerHub Image: https://hub.docker.com/r/anushreegm12/python-app


