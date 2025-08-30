# 🚀 CI/CD Pipeline with GitHub Actions & Docker (No Cloud Needed)

## 📌 Objective
Set up a full CI/CD pipeline that builds a Docker image, runs tests, and deploys locally using **Minikube** — without needing any cloud services.

---

## 🛠 Tools Used
- **GitHub Actions** – CI/CD workflow automation  
- **Docker & Docker Hub** – Containerization & image registry  
- **Minikube (Kubernetes)** – Local deployment  
- **Python Flask** – Sample application  

---

## 📂 Project Overview
This project demonstrates a complete CI/CD pipeline:

1. **Code pushed to GitHub** → triggers workflow  
2. **GitHub Actions** → installs dependencies, runs tests, builds Docker image, and pushes to Docker Hub  
3. **Minikube** → pulls the Docker image and deploys it locally  
4. **Service** → exposes the app at `http://127.0.0.1:<port>`  

✅ Result: Flask app accessible on local machine.

---

## 📁 Project Structure
ci-cd-demo/
├── .github/workflows/
│ └── ci-cd.yml # GitHub Actions workflow
├── app/
│ └── app.py # Flask app
├── Dockerfile
├── docker-compose.yml
--

---

## ▶️ How to Run Locally

1. Start Minikube:
```bash
minikube start
---
2. Apply deployment & service:
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
---
3. Open tunnel (keep this terminal open):
minikube tunnel
---
Access app in browser:
http://127.0.0.1:64812
You should see:
Hello from CI/CD with GitHub Actions & Docker!
----
📸 Screenshots

1. GitHub Actions Workflow Success

Proof that CI/CD ran successfully:


2. Docker Image on Docker Hub

Image pushed successfully:
👉 Docker Hub Link
https://hub.docker.com/repository/docker/divyanshush/ci-cd-demo/general


3. Flask App Running via Minikube

Application deployed and accessible:


✅ Deliverables

GitHub repo with workflows

Docker image link (Docker Hub repo
)

CI/CD workflow results (screenshot)

Screenshot of deployed app

 - `github-actions.png` → GitHub Actions success page  
   - `docker-hub.png` → Docker Hub repo page  
   - `minikube-app.png` → Browser window showing Flask app

