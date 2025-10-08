# Wanderlust: A MERN Stack DevOps Portfolio 🌍

A modern travel blog application originally created by **[Krishna Acharyaa](https://github.com/krishnaacharyaa/wanderlust)** and re-engineered by me to demonstrate advanced **DevOps proficiency**, focusing on containerization and cloud-native deployment principles.

## 🚀 My Goal: Structured DevOps Progression

The primary purpose of this repository is to showcase my skills in transforming a functional application into a robust, scalable, and fully automated deployment target. The project uses structured Git branches to illustrate a clear progression through different cloud-native technologies:

| Branch | Status | Focus | Description |
| :--- | :--- | :--- | :--- |
| `main` | Base Code | **Containerized Setup** | This branch serves as the base MERN application codebase, already configured with **Docker Compose** for immediate local launch. |
| `dockerized` | **Complete** | **Containerization** | Contains the comprehensive implementation of the Docker setup and optimization (multi-stage builds, minimal images). |
| `kubernetes` | *Upcoming* | **Orchestration** | Will demonstrate scalable deployment using Kubernetes YAMLs/Helm. |
| `terraform` | *Upcoming* | **Infrastructure as Code (IaC)** | Will demonstrate cloud resource provisioning and infrastructure management. |

---

## 🛠️ Local Setup (Docker Compose)

Your project requires **only Docker** and **Docker Compose (V2)** to be installed locally. All services (Backend, Frontend, MongoDB, Redis) are launched via containers, eliminating local dependency installations.

### 1. Clone the Repository

Clone the project and navigate into the directory.

```bash
git clone [https://github.com/Harshchrs/wanderlust-devops-portfolio.git](https://github.com/Harshchrs/wanderlust-devops-portfolio.git)
cd wanderlust-devops-portfolio
2. Configure Environment Variables
Create the necessary local configuration files for both the Backend and Frontend services from the provided samples.

Bash

cp backend/.env.sample backend/.env
cp frontend/.env.sample frontend/.env.local
3. Launch Services and Initialize Data
Run the stack and then inject the required sample data into the MongoDB container.

A. Launch Stack
Build and start all services (Backend, Frontend, Mongo, Redis) in the background.

Bash

docker compose up -d --build
B. Data Initialization
After the stack is running, execute the mongoimport command inside the running container to populate the database.

Bash

docker exec -it mongo mongoimport --db wanderlust --collection posts --file /data/sample_posts.json --jsonArray
4. Access the Application
The application is now fully running and initialized:

Frontend: Access the UI at http://localhost:5173

Backend API: Running internally on port 5000.

⚙️ Technology Stack
Component	Stack/Tool	My Focus
Original Codebase	MERN Stack (React, Node, Mongo, Express)	Leveraged for DevOps practice.
Containerization	Docker & Docker Compose	Implemented multi-service environment definition.
Database	MongoDB	Managed via persistent container volumes.
Caching	Redis	Integrated containerized caching solution.

Export to Sheets
⭐️ Show Your Support
I extend gratitude to Krishna Acharyaa for the foundation MERN project.

If you find my structural and technical contributions interesting, please consider starring the repository! Your support encourages me to keep building out the Kubernetes and Terraform stages.
