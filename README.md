# CI/CD Pipeline for Amazon ECS using GitHub Actions

## 🚀 Overview

This project demonstrates a complete CI/CD pipeline that automates deployment of a containerized Flask application to Amazon ECS using GitHub Actions and Amazon ECR.

The workflow simulates a production-grade deployment pipeline where every push to the `main` branch triggers an automated build, containerization, and deployment process.

---

## 🏗️ Architecture

```text
Git Push
   │
   ▼
GitHub Repository
   │
   ▼
GitHub Actions Runner (Ubuntu)
   │
   ├── Checkout Code
   ├── Build Docker Image
   ├── Authenticate AWS (via Secrets)
   ├── Push Image to Amazon ECR
   └── Deploy to Amazon ECS
   │
   ▼
Running Container on ECS Fargate


