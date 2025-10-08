🌍 Wanderlust: A MERN Stack DevOps Portfolio
A modern travel blog application originally created by Krishna Acharyaa and re-engineered by me to demonstrate advanced DevOps proficiency, focusing on containerization, orchestration, and cloud-native deployment principles.
————————————————————————————————————————
🚀 My Goal: Structured DevOps Progression
This repository showcases a structured evolution from a basic MERN app to a fully automated, cloud-ready deployment pipeline. Each Git branch represents a clear stage in this DevOps journey:
Branch	Status	Focus	Description
main	✅ Base Code	Containerized Setup	Base MERN codebase configured with Docker Compose for instant local deployment.
dockerized	✅ Complete	Containerization	Fully optimized Docker setup using multi-stage builds and minimal images.
kubernetes	🏗️ Upcoming	Orchestration	Will demonstrate scalable deployment using Kubernetes YAMLs / Helm charts.
terraform	🏗️ Upcoming	Infrastructure as Code (IaC)	Will showcase automated cloud provisioning via Terraform.
————————————————————————————————————————
🛠️ Local Setup (Docker Compose)
This project requires only Docker and Docker Compose (v2) — no manual Node, MongoDB, or Redis installations.
1️⃣ Clone the Repository
git clone https://github.com/Harshchrs/wanderlust-devops-portfolio.git
cd wanderlust-devops-portfolio
2️⃣ Configure Environment Variables
cp backend/.env.sample backend/.env
cp frontend/.env.sample frontend/.env.local
3️⃣ Launch Services and Initialize Data
A. Launch the Stack:

docker compose up -d --build
B. Initialize Sample Data:

docker exec -it mongo mongoimport --db wanderlust --collection posts --file /data/sample_posts.json --jsonArray
4️⃣ Access the Application
Frontend: http://localhost:5173
Backend API: http://localhost:5000
————————————————————————————————————————
⚙️ Technology Stack
Component	Stack / Tool	My Focus
Original Codebase	MERN Stack (Mongo, Express, React, Node)	Leveraged for DevOps experimentation
Containerization	Docker & Docker Compose	Multi-service orchestration and optimized builds
Database	MongoDB	Managed via persistent container volumes
Caching	Redis	Integrated containerized caching solution
————————————————————————————————————————
🧭 Future Roadmap
- [ ] Kubernetes deployment with Helm
- [ ] Terraform-based cloud provisioning
- [ ] CI/CD automation with GitHub Actions
- [ ] Monitoring setup using Prometheus + Grafana
————————————————————————————————————————
⭐️ Show Your Support
Huge thanks to Krishna Acharyaa for the original MERN foundation.

If you find my DevOps structure and implementation approach valuable — please consider starring this repository. Your support motivates me to continue building the upcoming Kubernetes and Terraform stages.
————————————————————————————————————————
Author: Harsh Chaurasia
📧 Connect on LinkedIn: https://www.linkedin.com/in/harshchrs/
📂 Repository: https://github.com/Harshchrs/wanderlust-devops-portfolio
