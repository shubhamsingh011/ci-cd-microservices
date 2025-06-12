# CI/CD Pipeline for Microservices

This project demonstrates a complete CI/CD pipeline for deploying microservices using **Jenkins**, **Docker**, and **Kubernetes**.

---

## 📦 Microservices

- `user-service`
- `order-service` (WIP – coming soon)

Each service has:
- Its own Dockerfile
- A Jenkinsfile for CI/CD
- Kubernetes deployment YAML files

---

## 🚀 Technologies Used

| Tool/Technology  | Purpose                                 |
|------------------|------------------------------------------|
| Git & GitHub     | Version control and repository hosting   |
| Jenkins          | CI/CD automation                         |
| Docker           | Containerization of microservices        |
| Kubernetes       | Container orchestration (Minikube/EKS)   |
| Maven/Gradle     | Java build tools                         |

---

## 🧱 Project Structure

ci-cd-microservices/
├── user-service/
│ ├── Dockerfile
│ ├── Jenkinsfile
│ ├── k8s/
│ │ └── deployment.yaml
│ └── src/
│ └── (source code or dummy jar)
└── order-service/
└── (coming soon)

yaml
Copy
Edit

---

## 🔁 CI/CD Pipeline Workflow

1. **Code Commit** – Push code to GitHub.
2. **Jenkins Trigger** – Jenkins is triggered via webhook.
3. **Docker Build** – Jenkins builds the Docker image.
4. **Push to DockerHub** – Jenkins pushes the image to a registry.
5. **Kubernetes Deploy** – Jenkins deploys the updated image to K8s cluster.

---

## ⚙️ Jenkins Pipeline (user-service)

The pipeline performs:
- Checkout from GitHub
- Docker image build & push
- Kubernetes deployment using `kubectl`

See [`user-service/Jenkinsfile`](./user-service/Jenkinsfile) for details.

---

## 🛠️ Prerequisites

- Jenkins with Docker and K8s CLI plugins
- DockerHub account
- Kubernetes cluster (Minikube, Docker Desktop, or AWS EKS)
- GitHub Webhook connected to Jenkins

---

## 📸 Screenshots (optional)

_Add screenshots of Jenkins pipeline, DockerHub, K8s dashboard, etc._

---

## 📌 TODO

- Add `order-service` and other microservices
- Helm-based deployment
- GitOps using ArgoCD (future enhancement)

---

## 👤 Author

**Shubham Singh**  
DevOps Engineer | Automation Enthusiast

---

## 📬 Contact

Feel free to reach out on [LinkedIn](https://www.linkedin.com/in/shubham-singh-2a2572170/) or raise an issue!

