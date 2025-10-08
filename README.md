Wanderlust: A MERN Stack DevOps Portfolio 🌍
A modern travel blog application originally created by Krishna Acharyaa (Link to original repo if known) and re-engineered by me to demonstrate advanced DevOps proficiency, focusing on containerization and cloud-native deployment principles.

🚀 My Goal: Structured DevOps Progression
The primary purpose of this repository is to showcase my skills in transforming a functional application into a robust, scalable, and fully automated deployment target. The project uses structured Git branches to illustrate a clear progression through different cloud-native technologies:

Branch	Status	Focus	Description
main	Base Code	Containerized Setup	This branch serves as the base MERN application codebase, already configured with Docker Compose for immediate local launch.
dockerized	Complete	Containerization	Contains the comprehensive implementation of the Docker setup and optimization (multi-stage builds, minimal images).
kubernetes	Upcoming	Orchestration	Will demonstrate scalable deployment using Kubernetes YAMLs/Helm.
terraform	Upcoming	Infrastructure as Code (IaC)	Will demonstrate cloud resource provisioning and infrastructure management.

Export to Sheets
🛠️ Local Setup (Docker Compose)
Your project requires only Docker and Docker Compose (V2) to be installed locally. All services (Backend, Frontend, MongoDB, Redis) are launched via containers, eliminating local dependency installations.

1. Clone the Repository
Bash

git clone https://github.com/Harshchrs/wanderlust-devops-portfolio.git
cd wanderlust-devops-portfolio
2. Configure and Launch Services
Environment Setup: Create the necessary configuration files.

Bash

cp backend/.env.sample backend/.env
cp frontend/.env.sample frontend/.env.local
Launch Stack: Build and start all services in the background.

Bash

docker compose up -d --build
Data Initialization: After the stack is running, initialize the database with sample data.

Bash

# Execute mongoimport inside the running Mongo container
docker exec -it mongo mongoimport --db wanderlust --collection posts --file /data/sample_posts.json --jsonArray
3. Access the Application
Frontend: Access the UI at http://localhost:5173

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
