# 🚀 CI/CD Pipeline for a Java Application

![CI](https://img.shields.io/badge/CI-Jenkins-blue?logo=jenkins)
![CD](https://img.shields.io/badge/CD-Kubernetes-blue?logo=kubernetes)
![Docker](https://img.shields.io/badge/Container-Docker-blue?logo=docker)
![Platform](https://img.shields.io/badge/Platform-Minikube-orange)
![Language](https://img.shields.io/badge/Language-Java-red?logo=java)
![Repo](https://img.shields.io/badge/GitHub-Repository-black?logo=github)

---

## 📌 Overview

This project demonstrates a complete **end-to-end CI/CD pipeline** built using **Jenkins Pipeline (Jenkinsfile)** to automate:

- Building a Java application  
- Creating Docker images  
- Pushing images to Docker Hub  
- Deploying the application to Kubernetes (Minikube)  

---

## 🏗️ Architecture Diagram

```mermaid
flowchart LR
    A[GitHub Repo] -->|Code Push| B[Jenkins Pipeline]
    B --> C[Build Java App]
    C --> D[Build Docker Images]
    D --> E[Push to Docker Hub]
    E --> F[Deploy to Kubernetes]
    F --> G[Minikube Cluster]
    G --> H[Application Running]
````

---

## 🔧 Tech Stack

* Jenkins (Pipeline as Code - Jenkinsfile)
* Docker
* Kubernetes (Minikube)
* GitHub
* Java Application

---

## 🔄 Pipeline Stages

1. Pull the source code and detect changes
2. Build the application
3. Build application and database Docker images
4. Push images to Docker Hub
5. Deploy to Kubernetes

---

## 💡 Key Challenges & Fixes

* **Docker Build Failure (DNS issue)**
  ✔ Fixed by configuring Docker DNS/network

* **Kubernetes Authentication Issue**
  ✔ Fixed by providing kubeconfig for Jenkins

* **Cluster Connectivity Issue**
  ✔ Fixed by recreating Minikube cluster

* **Permission Issue on Certificates**
  ✔ Fixed by adjusting Linux file permissions

* **Application Not Accessible**
  ✔ Fixed by correcting Service `targetPort`

---

## 📊 Key Learnings

* Most CI/CD failures are environment-related, not tool-related
* Linux permissions are critical in DevOps
* Kubernetes networking requires correct port mapping
* Troubleshooting step-by-step is essential

---

# 📁 Project as a Case Study (Portfolio Section)

## 🎯 Objective

Automate the deployment of a Java application using a full CI/CD pipeline from code commit to Kubernetes deployment.

---

## 🧩 Problem

Manual deployment processes are:

* Time-consuming
* Error-prone
* Not scalable

---

## ⚙️ Solution

Implemented a CI/CD pipeline using Jenkins to:

* Automate build and test
* Containerize the application using Docker
* Push images to Docker Hub
* Deploy automatically to Kubernetes

---

## 🚀 Outcome

* Fully automated deployment pipeline
* Faster and repeatable deployments
* Reduced human error
* Hands-on experience with real DevOps challenges
<img width="975" height="515" alt="image" src="https://github.com/user-attachments/assets/d2da9aa3-00fa-434e-bd40-fbcd60bb6377" />


<img width="975" height="518" alt="image" src="https://github.com/user-attachments/assets/fd5e5b1b-4a8f-49fb-a944-a73c010dc755" />
