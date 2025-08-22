# Kubernetes Autoscaling with HPA 🚀

## Project Overview
This project demonstrates **Horizontal Pod Autoscaling (HPA)** on Kubernetes using a CPU-intensive Flask application.  
The app is deployed with resource limits, exposed via a service, and automatically scales based on CPU utilization.

## ⚙️ Features
- Flask app with CPU-intensive endpoint
- Dockerized application
- Kubernetes Deployment, Service, and HPA
- GitHub Actions CI/CD Pipeline (build → push → deploy)

## 🛠️ How to Run
1. Clone this repo
2. Update dockerhub username in `deployment.yaml`
3. Push code to `main` branch → GitHub Actions will build & deploy automatically
4. Check HPA:
   ```bash
   kubectl get hpa
   kubectl get pods
