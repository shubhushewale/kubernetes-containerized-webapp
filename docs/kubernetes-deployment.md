\# Kubernetes Deployment



\## Overview



Deployed the Dockerized Nginx web application on a Kubernetes cluster.



\## Deployment



Created a Kubernetes Deployment with 3 replicas.



The Deployment manages a ReplicaSet that maintains the desired number of application Pods.



\## Container Image



Docker image:



shubhamdocker2025/kubernetes-webapp:v1



The container image is stored in Docker Hub.



\## Self-Healing Test



Manually deleted one application Pod.



The ReplicaSet detected that the actual Pod count was lower than the desired replica count and automatically created a replacement Pod.



\## Service



Created a NodePort Service.



The Service uses the label selector:



app: kubernetes-webapp



The Service forwards traffic to application Pods on port 80.



\## Verification



Verified:



\- Deployment status

\- ReplicaSet

\- 3 running Pods

\- Kubernetes self-healing

\- Service endpoints

\- Application access using port forwarding

