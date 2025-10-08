# 🌍 Wanderlust: A DevOps Portfolio Project

A modern travel blog application originally created by **[Krishna Acharyaa](https://github.com/krishnaacharyaa/wanderlust)** and re-engineered by me to demonstrate advanced DevOps skills—containerization, orchestration, and infrastructure automation.

---

## 🚀 Project Overview

The goal is to take a simple MERN application and progressively transform it into a production-grade, cloud-native deployment, documenting each stage using separate Git branches.

| Branch | Status | Focus | Description |
| :--- | :--- | :--- | :--- |
| `main` | ✅ Complete | Containerized Setup | Base MERN app integrated with Docker Compose. |
| `dockerized` | ✅ Complete | Containerization | Optimized multi-stage builds and minimal images for services. |
| `kubernetes` | 🕒 Upcoming | Orchestration | Will include scalable deployment with Kubernetes/Helm. |
| `terraform` | 🕒 Upcoming | Infrastructure as Code | Will include AWS provisioning and IaC workflows. |

---

## 🛠️ Local Setup (Docker Compose)

**Requirements:** Docker and Docker Compose v2. No need to install Node, MongoDB, or Redis locally.

1. Clone Repository
```bash
git clone https://github.com/Harshchrs/wanderlust-devops-portfolio.git
cd wanderlust-devops-portfolio
```
2. Configure Environment Variables
```bash
cp backend/.env.sample backend/.env
cp frontend/.env.sample frontend/.env.local
```
3. Launch Stack
```bash
docker compose up -d --build
```
4. Initialize Data
```bash
docker exec -it mongo mongoimport --db wanderlust --collection posts --file /data/sample_posts.json --jsonArray
```
5. Access Application
Frontend → http://localhost:5173

Backend API → runs internally on port 5000.
⚙️ Tech Stack
• MERN Stack – base web app.
• Docker & Compose – containerized microservices.
• MongoDB & Redis – database and caching containers.
• Kubernetes (upcoming) – orchestration & scaling.
• Terraform (upcoming) – AWS infrastructure provisioning.
• Jenkins, ArgoCD, Prometheus (planned) – CI/CD & monitoring.
⭐ Acknowledgment
Thanks to [Krishna Acharyaa](https://github.com/krishnaacharyaa/wanderlust) for the original base project. If you find my DevOps adaptation valuable, consider starring the repository — it helps support future stages like Kubernetes & Terraform.

