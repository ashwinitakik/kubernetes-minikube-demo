# Kubernetes Minikube Demo

This project demonstrates how to deploy and manage a simple application on a local Kubernetes cluster using **Minikube**.

---

## 🧩 Tools Used
- Minikube  
- kubectl  
- Docker  

---

## ⚙️ Steps Performed
1. Installed Docker, Minikube, kubectl.
2. Started local Kubernetes cluster using Minikube.
3. Created `deployment.yaml` for Nginx app.
4. Created `service.yaml` to expose app using NodePort.
5. Verified pods and services using `kubectl get pods` and `kubectl get svc`.
6. Scaled deployment to multiple replicas.
7. Viewed app in browser using `minikube service nginx-service`.

---

## 📸 Screenshots
| Description | Screenshot |
|--------------|-------------|
| Pods running | ![Pods](screenshots/pods.png) |
| Services | ![Services](screenshots/services.png) |
| Browser output | ![Browser](screenshots/browser.png) |

---

## 🧹 Cleanup
```bash
kubectl delete -f deployment.yaml
kubectl delete -f service.yaml
minikube stop
minikube delete
