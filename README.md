# 🚀 Cloud-Native CI/CD Platform using AWS, K3s & GitHub Actions

## 📌 Overview

This project demonstrates an **end-to-end cloud-native CI/CD pipeline** using **AWS EC2, Kubernetes (K3s), GitHub Actions, Docker, and Secrets Management**.

It shows how application code changes are automatically:
- Built
- Containerized
- Deployed
- Updated on a Kubernetes cluster

using modern DevOps practices.

This project is designed as a **hands-on DevOps learning and portfolio project** simulating real-world CI/CD workflows.

---

## 🧱 High-Level Architecture

Developer
|
| Git Push
v
GitHub Repository
|
| Triggers
v
GitHub Actions (CI/CD Pipeline)
|
| Build Docker Image
| Push Image
v
Container Registry
|
| Deploy
v
AWS EC2
|
| Running
v
Kubernetes (K3s Cluster)
|
| Manages
v
Application Pods


---

## 🧠 Workflow Explanation

1. Developer pushes code to GitHub repository
2. GitHub Actions pipeline is triggered automatically
3. Pipeline:
   - Builds Docker image
   - Pushes image to registry
   - Deploys application to Kubernetes (K3s) cluster
4. Kubernetes performs:
   - Rolling update
   - Self-healing
   - Container orchestration

---

## 🛠️ Technologies Used

- **Cloud:** AWS EC2
- **CI/CD:** GitHub Actions
- **Containers:** Docker
- **Orchestration:** Kubernetes (K3s)
- **OS:** Linux
- **Secrets Management:** GitHub Secrets
- **Version Control:** Git & GitHub

---

## ✨ Features

- Fully automated CI/CD pipeline
- Containerized application deployments
- Kubernetes-based orchestration using K3s
- Secure secrets handling using GitHub Secrets
- Rolling updates and automated redeployments
- Cloud-hosted infrastructure on AWS EC2

---

## 🔐 Secrets Management

Sensitive information such as:
- Server IP
- SSH keys
- Credentials

are stored securely using **GitHub Repository Secrets** and injected into the pipeline at runtime.

---

## 🧰 Prerequisites

- AWS Account
- Linux EC2 Instance
- Docker installed
- K3s installed on EC2
- GitHub Account
- Basic knowledge of Git, Docker, Kubernetes

---

## ⚙️ Setup Steps (High Level)

1. Launch EC2 instance on AWS
2. Install Docker and K3s on the server
3. Clone this repository
4. Configure GitHub Secrets:
   - Server IP
   - SSH Key
   - Any required credentials
5. Push code to GitHub
6. GitHub Actions pipeline will trigger automatically

---

## ▶️ How to Run

```bash
git clone https://github.com/sairohith10/devops--practice.git
cd devops--practice
git push origin main
