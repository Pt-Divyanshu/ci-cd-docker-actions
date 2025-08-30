# 🚀 CI/CD Pipeline with GitHub Actions, Docker & Kubernetes (Minikube)

This project demonstrates a **CI/CD pipeline** where a Flask application is built, tested, containerized with **Docker**, and deployed on a local **Kubernetes cluster** using **Minikube**.  

---

## 📌 Features
- ✅ GitHub Actions workflow for CI/CD  
- ✅ Docker image build & push to Docker Hub  
- ✅ Kubernetes Deployment & Service for Flask app  
- ✅ Access application via Minikube NodePort  

---

## 🛠️ Tools & Technologies
- **GitHub Actions** – CI/CD pipeline automation  
- **Docker** – Containerization  
- **Docker Hub** – Image registry  
- **Kubernetes (Minikube)** – Container orchestration  
- **Flask** – Python web framework  

---

## ⚙️ Workflow
1. Code is pushed to GitHub.  
2. GitHub Actions builds Docker image & pushes it to Docker Hub.  
3. Kubernetes Deployment & Service files are applied.  
4. Flask app becomes available via Minikube service.  

---

## 📂 Project Structure
ci-cd-docker-actions/
├── app.py
├── requirements.txt
├── Dockerfile
├── docker-compose.yml
├── .github/workflows/ci-cd.yml
├── k8s/
│ ├── deployment.yml
│ └── service.yml
---

---

##  How to Run Locally

### Step 1: Clone the repo
git clone https://github.com/Pt-Divyanshu/ci-cd-docker-actions.git
cd ci-cd-docker-actions
2️⃣ Run with Minikube
minikube start
kubectl apply -f k8s/deployment.yml
kubectl apply -f k8s/service.yml
kubectl get pods
kubectl get svc

3️⃣ Access Flask App
minikube service flask-app


Example:
👉 http://127.0.0.1:64812

📸 Screenshots
### 1. Application Output
The deployed Flask app running in the browser:

![Sample App Output](smaple%20app.png)

---

### 2. Docker Images
Docker Desktop showing the built image and its details:

![Docker Images](Docker%20image.png)

---

### 3. GitHub Actions Workflow Success
Successful CI/CD pipeline execution on GitHub:

![GitHub Workflows](github%20workflows.png)

---

🎯 Output

When you open the app in browser, you’ll see:

Hello from CI/CD with GitHub Actions & Docker!

👨‍💻 Author

Divyanshu Sharma
----


