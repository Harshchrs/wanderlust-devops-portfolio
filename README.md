# Wanderlust DevOps Portfolio 🌍

A modern travel blog application built on the **MERN Stack** (MongoDB, Express, React, Node.js) and re-engineered to demonstrate end-to-end DevOps skills, focusing on containerization and cloud-native deployment principles.

---

## 🚀 DevOps Showcase

This project uses Git branches to illustrate a clear, structured progression through different cloud technologies:

| Branch | Status | Focus | Key Files |
| :--- | :--- | :--- | :--- |
| `main` | Base Code | Clean MERN application codebase. | `package.json`, `backend/server.ts` |
| `dockerized` | **Complete** | **Containerization** using Docker and Docker Compose for a consistent local environment. | `docker-compose.yml`, `backend/Dockerfile` |
| `kubernetes` | *Upcoming* | Orchestration using Kubernetes for scalable, highly available deployment. | `*.yaml`, `Helm Charts` |
| `terraform` | *Upcoming* | Infrastructure as Code (IaC) for deploying and managing cloud resources. | `*.tf` |

---

## 🛠️ Local Setup (Dockerized)

To run the full application stack locally using the `dockerized` branch:

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/Harshchrs/wanderlust-devops-portfolio
    cd wanderlust
    ```
2.  **Checkout the Docker Branch:**
    ```bash
    git switch dockerized
    ```
3.  **Configure Environment:** Create the necessary configuration files.
    ```bash
    cp backend/.env.sample backend/.env
    cp frontend/.env.sample frontend/.env.local
    ```
4.  **Launch Services:**
    ```bash
    docker compose up -d --build
    ```
    * **Frontend:** Accessible at `http://localhost:5173`
    * **Backend API:** Accessible at `http://localhost:5000`

---

## ⚙️ Technology Stack

| Component | Stack/Tool | Description |
| :--- | :--- | :--- |
| **Frontend** | React, TypeScript, Tailwind CSS | Modern, component-based UI. |
| **Backend** | Node.js, Express.js, TypeScript | RESTful API server. |
| **Database** | MongoDB | Persistent data storage. |
| **Caching** | Redis | Session and caching management. |
| **Containerization** | **Docker** & **Docker Compose** | Defines and manages the multi-service application environment. |

---

## ⭐️ Show Your Support

If you find this project interesting, please consider starring the repository! It encourages me to keep building out the Kubernetes and Terraform stages.
