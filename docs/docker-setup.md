\# Docker Setup



\## Application



Created a static HTML web application.



\## Docker Image



Used Nginx Alpine as the base image.



Docker image:



kubernetes-webapp:v1



\## Docker Build



docker build -t kubernetes-webapp:v1 .



\## Container Deployment



docker run -d --name kubernetes-webapp-container -p 8080:80 kubernetes-webapp:v1



\## Verification



The application was successfully accessed using localhost on port 8080.



Container logs were verified using the docker logs command.

