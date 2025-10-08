# 🌍 Wanderlust: A MERN Stack DevOps Portfolio

A modern travel blog application originally created by **[Krishna Acharyaa](https://github.com/krishnaacharyaa/wanderlust)** and re-engineered by me to demonstrate advanced **DevOps proficiency**, focusing on containerization, orchestration, and cloud-native deployment principles.

---

## 🚀 My Goal: Structured DevOps Progression

This repository showcases a structured evolution from a basic MERN app to a **fully automated, cloud-ready deployment pipeline**.  
Each Git branch represents a key stage in this DevOps transformation:

| Branch | Status | Focus | Description |
| :--- | :--- | :--- | :--- |
| `main` | ✅ Base Code | **Containerized Setup** | Base MERN codebase configured with **Docker Compose** for instant local deployment. |
| `dockerized` | ✅ Complete | **Containerization** | Fully optimized Docker setup using multi-stage builds and minimal images. |
| `kubernetes` | 🏗️ Upcoming | **Orchestration** | Will demonstrate scalable deployment using **Kubernetes YAMLs / Helm charts**. |
| `terraform` | 🏗️ Upcoming | **Infrastructure as Code (IaC)** | Will demonstrate automated cloud provisioning via **Terraform**. |

---

## 🛠️ Local Setup (Docker Compose)

This project requires **only Docker** and **Docker Compose (v2)** — no need to install Node, MongoDB, or Redis locally.

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Harshchrs/wanderlust-devops-portfolio.git
cd wanderlust-devops-portfolio
2️⃣ Configure Environment Variables
Copy the provided sample environment files:

bash
Copy code
cp backend/.env.sample backend/.env
cp frontend/.env.sample frontend/.env.local
Edit these files if needed to match your local setup (Mongo/Redis configs, ports, etc.).

3️⃣ Launch Services and Initialize Data
A. Launch the Stack
Build and start all services (Backend, Frontend, MongoDB, Redis):

bash
Copy code
docker compose up -d --build
B. Initialize Sample Data
Once containers are running, import the sample data into MongoDB:

bash
Copy code
docker exec -it mongo mongoimport --db wanderlust --collection posts --file /data/sample_posts.json --jsonArray
4️⃣ Access the Application
Service	URL	Description
Frontend (React)	http://localhost:5173	User interface for the blog
Backend (Express API)	http://localhost:5000	Runs internally within Docker network

⚙️ Technology Stack
Component	Stack / Tool	My Focus
Original Codebase	MERN Stack (Mongo, Express, React, Node)	Leveraged for DevOps experimentation
Containerization	Docker & Docker Compose	Multi-service orchestration, optimized builds
Database	MongoDB	Persistent containerized data storage
Caching	Redis	Integrated caching within container setup

🧭 Future Roadmap
 Kubernetes deployment with Helm

 Terraform-based AWS provisioning

 CI/CD automation with GitHub Actions

 Monitoring setup using Prometheus + Grafana

⭐️ Show Your Support
Huge thanks to Krishna Acharyaa for the original MERN project foundation.

If you find my DevOps structure and implementation approach valuable —
please consider starring the repository! Your support helps me continue building out the Kubernetes and Terraform stages.

Author: Harsh Chaurasia
📧 Reach me on LinkedIn
📂 Repository: wanderlust-devops-portfolio

yaml
Copy code

---

Would you like me to make it *slightly more portfolio-marketing* (like a personal project pitch for recruiters) — or keep it *strictly technical-documentation style* for engineers reading the repo?






You said:
can you write it in one go so i can just copy paste


ChatGPT said:
Sure — here’s the final polished README you can copy-paste directly into GitHub.
Perfectly formatted, consistent spacing, links preserved, and professional tone.

markdown
Copy code
# 🌍 Wanderlust: A MERN Stack DevOps Portfolio

A modern travel blog application originally created by **[Krishna Acharyaa](https://github.com/krishnaacharyaa/wanderlust)** and re-engineered by me to demonstrate advanced **DevOps proficiency**, focusing on containerization, orchestration, and cloud-native deployment principles.

---

## 🚀 My Goal: Structured DevOps Progression

This repository showcases a structured evolution from a basic MERN app to a **fully automated, cloud-ready deployment pipeline**.  
Each Git branch represents a clear stage in this DevOps journey:

| Branch | Status | Focus | Description |
| :--- | :--- | :--- | :--- |
| `main` | ✅ Base Code | **Containerized Setup** | Base MERN codebase configured with **Docker Compose** for instant local deployment. |
| `dockerized` | ✅ Complete | **Containerization** | Fully optimized Docker setup using multi-stage builds and minimal images. |
| `kubernetes` | 🏗️ Upcoming | **Orchestration** | Will demonstrate scalable deployment using **Kubernetes YAMLs / Helm charts**. |
| `terraform` | 🏗️ Upcoming | **Infrastructure as Code (IaC)** | Will showcase automated cloud provisioning via **Terraform**. |

---

## 🛠️ Local Setup (Docker Compose)

This project requires **only Docker** and **Docker Compose (v2)** — no manual Node, MongoDB, or Redis installations.

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Harshchrs/wanderlust-devops-portfolio.git
cd wanderlust-devops-portfolio
2️⃣ Configure Environment Variables
Copy the sample configuration files for both Backend and Frontend:

bash
Copy code
cp backend/.env.sample backend/.env
cp frontend/.env.sample frontend/.env.local
Edit them if needed to match your local configuration.

3️⃣ Launch Services and Initialize Data
A. Launch the Stack
Build and start all services (Backend, Frontend, MongoDB, Redis):

bash
Copy code
docker compose up -d --build
B. Initialize Sample Data
Once containers are running, import the sample dataset into MongoDB:

bash
Copy code
docker exec -it mongo mongoimport --db wanderlust --collection posts --file /data/sample_posts.json --jsonArray
4️⃣ Access the Application
Service	URL	Description
Frontend (React)	http://localhost:5173	User interface for the blog
Backend (Express API)	http://localhost:5000	Internal API endpoint within Docker network

⚙️ Technology Stack
Component	Stack / Tool	My Focus
Original Codebase	MERN Stack (Mongo, Express, React, Node)	Leveraged for DevOps experimentation
Containerization	Docker & Docker Compose	Multi-service orchestration and optimized builds
Database	MongoDB	Managed via persistent container volumes
Caching	Redis	Integrated containerized caching solution

🧭 Future Roadmap
 Kubernetes deployment with Helm

 Terraform-based cloud provisioning

 CI/CD automation with GitHub Actions

 Monitoring setup using Prometheus + Grafana

⭐️ Show Your Support
Huge thanks to Krishna Acharyaa for the original MERN foundation.

If you find my DevOps structure and implementation approach valuable —
please consider starring this repository ⭐️
Your support motivates me to continue building the upcoming Kubernetes and Terraform stages.

Author: Harsh Chaurasia
📂 Repository: wanderlust-devops-portfolio
