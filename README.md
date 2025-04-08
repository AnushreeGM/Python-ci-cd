# CI/CD Pipeline: Docker, Kubernetes, and Jenkins Integration

## 🚀 Objective

This project demonstrates the automation of a complete CI/CD pipeline using Docker, Kubernetes, and Jenkins for a sample application. It includes steps to containerize the app, deploy it to Kubernetes, and automate the workflow using Jenkins.

---

## 📦 Tech Stack

- Docker
- Kubernetes (Minikube or Managed Cluster)
- Jenkins
- GitHub
- DockerHub
- Sample App: [Python / Node.js / Java - specify your stack]

---

## ✅ Tasks Completed

### 🔹 Question 1: Containerize and Push the Application

- Forked and cloned the sample application.
- Packaged the application appropriately (e.g., JAR for Java, ZIP for Node.js/Python).
- Created a Dockerfile to containerize the application.
- Built the Docker image and pushed it to DockerHub.

#### DockerHub Link:
[👉 Docker Image on DockerHub](https://hub.docker.com/r/yourusername/your-image-name)

---

### 🔹 Question 2: Kubernetes Deployment and Service Exposure

- Created `deployment.yaml` to deploy the Docker image.
- Created `service.yaml` to expose the application via NodePort.
- Applied the YAMLs using `kubectl apply -f`.
- Verified the deployment and accessed the app using public IP and NodePort.

---

### 🔹 Question 3: Scale the Deployment

- Scaled the deployment to 3 replicas using:

```bash
kubectl scale deployment your-deployment-name --replicas=3
