\# Kubernetes Containerized Web Application



\## 📌 Project Overview



This project demonstrates the deployment of a Dockerized web application on a Kubernetes cluster using production-oriented Kubernetes resources.



The application is containerized using Docker, pushed to Docker Hub, and deployed to Kubernetes using a Deployment and Service. The project also demonstrates important Kubernetes concepts such as ConfigMaps, Secrets, Health Probes, Resource Requests \& Limits, Rolling Updates, Rollbacks, Scaling, Node Affinity, and Self-Healing.



\---



\## 🏗️ Architecture



!\[Architecture](architecture/project2-architecture.png)



\---



\## 🚀 Technologies Used



\- Docker

\- Docker Hub

\- Kubernetes

\- Nginx

\- YAML

\- Git

\- GitHub



\---



\## ☸️ Kubernetes Resources Used



\- Namespace

\- Deployment

\- ReplicaSet

\- Pods

\- Service (NodePort)

\- ConfigMap

\- Secret

\- Liveness Probe

\- Readiness Probe

\- Resource Requests

\- Resource Limits

\- Node Affinity



\---



\## ✨ Features



\- Dockerized Nginx Web Application

\- Kubernetes Deployment

\- Multiple Replica Pods

\- NodePort Service

\- ConfigMap for application configuration

\- Secret for sensitive data

\- Resource Requests \& Limits

\- Liveness \& Readiness Probes

\- Rolling Updates

\- Rollback Support

\- Horizontal Scaling

\- Self-Healing Pods

\- Node Affinity Scheduling

\- GitHub Documentation



\---



\## 📁 Project Structure



```text

kubernetes-containerized-webapp/

│

├── app/

│   ├── Dockerfile

│   └── index.html

│

├── architecture/

│   └── project2-architecture.png

│

├── docs/

│   ├── docker-setup.md

│   ├── kubernetes-deployment.md

│   └── configmap-secret.md

│

├── k8s/

│   ├── namespace.yaml

│   ├── deployment.yaml

│   ├── service.yaml

│   ├── configmap.yaml

│   └── secret.yaml

│

├── screenshots/

│

└── README.md

```



\---



\# 📦 Docker



\## Build Docker Image



```bash

docker build -t kubernetes-webapp:v1 .

```



\## Tag Image



```bash

docker tag kubernetes-webapp:v1 <dockerhub-username>/kubernetes-webapp:v1

```



\## Push Image



```bash

docker push <dockerhub-username>/kubernetes-webapp:v1

```



\---



\# ☸️ Kubernetes Deployment



\## Create Namespace



```bash

kubectl apply -f k8s/namespace.yaml

```



\## Deploy Application



```bash

kubectl apply -f k8s/

```



\## Verify Resources



```bash

kubectl get all

```



\---



\# 🔍 Verification Commands



\## Check Deployments



```bash

kubectl get deployments

```



\## Check Pods



```bash

kubectl get pods

```



\## Check Services



```bash

kubectl get svc

```



\## Check ConfigMaps



```bash

kubectl get configmap

```



\## Check Secrets



```bash

kubectl get secret

```



\---



\# 📈 Scaling



Increase replicas



```bash

kubectl scale deployment kubernetes-webapp-deployment --replicas=5

```



Decrease replicas



```bash

kubectl scale deployment kubernetes-webapp-deployment --replicas=2

```



\---



\# 🔄 Rolling Update



```bash

kubectl set image deployment/kubernetes-webapp-deployment \\

kubernetes-webapp=<dockerhub-username>/kubernetes-webapp:v2

```



\---



\# ⏪ Rollback



```bash

kubectl rollout undo deployment/kubernetes-webapp-deployment

```



\---



\# ❤️ Health Checks



This project demonstrates:



\- Liveness Probe

\- Readiness Probe



These probes help Kubernetes detect unhealthy containers and ensure only healthy Pods receive traffic.



\---



\# 📊 Resource Management



Configured:



\- CPU Requests

\- CPU Limits

\- Memory Requests

\- Memory Limits



This helps Kubernetes schedule Pods efficiently and prevents resource overconsumption.



\---



\# 🛠️ Self-Healing



The project demonstrates Kubernetes self-healing.



If a Pod is manually deleted:



```bash

kubectl delete pod <pod-name>

```



Kubernetes automatically creates a new Pod to maintain the desired replica count.



\---



\# 📸 Screenshots



Project includes screenshots for:



\- Docker Image Build

\- Docker Hub Repository

\- Kubernetes Cluster

\- Running Pods

\- Deployment

\- Service

\- ConfigMap

\- Secret

\- Rolling Update

\- Rollback

\- Scaling

\- Self-Healing

\- Running Application



\---



\# 🎯 Key Learnings



Through this project, I gained hands-on experience with:



\- Docker Image Creation

\- Docker Hub

\- Kubernetes Deployments

\- ReplicaSets

\- Pods

\- Services

\- ConfigMaps

\- Secrets

\- Resource Requests \& Limits

\- Liveness \& Readiness Probes

\- Rolling Updates

\- Rollbacks

\- Scaling

\- Node Affinity

\- Kubernetes Self-Healing

\- GitHub Project Documentation



\---



\# 👨‍💻 Author



\*\*Shubham Shewale\*\*



\*\*LinkedIn\*\*



https://www.linkedin.com/in/shubham-shewale-6aa444224



\*\*GitHub\*\*



https://github.com/shubhushewale



\---



\## ⭐ If you found this project helpful, consider giving it a star!

