# README

# Rails + PostgreSQL CI/CD with Docker, Kubernetes, Tekton and argoCD

This repository demonstrates a CI/CD pipeline for a Ruby on Rails application using Docker, Kubernetes, and Tekton Pipelines. The application is deployed in a Kubernetes cluster using manifests and built into a container image using Tekton's Kaniko executor.

---

# Stack Used

- Ruby on Rails
- PostgreSQL
- Docker
- Kubernetes (via Minikube)
- Tekton Pipelines

---

# Repository Structure

├── Dockerfile
├── kubernetes/
│ ├── deployment.yaml
│ ├── postgres-deployment.yaml
│ ├── service.yaml
├── tekton/
│ ├── pipeline.yaml
│ ├── pipelinerun.yaml
│ ├── kaniko-task.yaml
│ ├── git-clone-task.yaml
│ └── serviceaccount.yaml
└── README.md


---

 What Has Been Implemented

- Containerized a Ruby on Rails application using a Dockerfile.
- Created Kubernetes manifests to deploy the Rails app and PostgreSQL.
- Set up Tekton Pipelines for CI/CD:
  - Clones the Git repository.
  - Builds the Docker image using **Kaniko**.
  - Pushes the image to Docker Hub.
- Exposed the Rails application using Kubernetes `NodePort` service on port `44301`.
- Verified successful pipeline execution using `tkn` CLI and browser access to the app.

---
NOTE

* i have not worked on argoCD yet cause i have never worked on it but i am currentlly working on it. i am submitting the task for now incomplete beacause my deadline is already over due to lack of time to work on this task as i am working in an organisation. so, hope you understand and i really want this job as i loved the task and i learned alot from it so i'll definatelly learn more while working there.

* thank you for the oppertunity.

* regards,
  shreyansh rajyaguru.
