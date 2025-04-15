# K8s Flask Demo

This project demonstrates how to containerize a simple Flask web app and deploy it to a Kubernetes cluster using Minikube.

Files

- `app.py`: Python Flask app
- `requirements.txt`: Dependencies
- `Dockerfile`: Docker image setup
- `deployment.yaml`: Kubernetes Deployment config
- `service.yaml`: Kubernetes Service (NodePort)

## 🚀 How to Deploy

1. **Start Minikube**  
   `minikube start`

2. **Use Minikube Docker**  
   `minikube docker-env` → then `SET` values on Windows CMD

3. **Build Docker Image**  
   `docker build -t my-k8s-app .`

4. **Deploy to Kubernetes**  
   `kubectl apply -f deployment.yaml`

5. **Create Service**  
   `kubectl apply -f service.yaml`

6. **Access the App**  
   `minikube service my-k8s-service`  
   or go to `http://localhost:30007`

