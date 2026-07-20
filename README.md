# CI/CD Pipeline for Amazon ECS using GitHub Actions

## Project Overview

Production-style CI/CD pipeline that automates the build, containerization, and deployment of a Flask application to Amazon ECS using GitHub Actions and Amazon ECR.

## Project Goal

Demonstrate an automated deployment pipeline following modern DevOps practices with continuous integration and continuous delivery on AWS.

## Architecture

```text
Developer
      │
      ▼
GitHub Repository
      │
      ▼
GitHub Actions
      │
      ├────────► Build Docker Image
      ├────────► Authenticate to AWS
      ├────────► Push Image to Amazon ECR
      └────────► Deploy to Amazon ECS
                    │
                    ▼
             ECS Fargate Service
```

## Technologies

- GitHub Actions
- Docker
- Amazon ECS
- Amazon ECR
- AWS IAM
- Flask

## Features

- Automated CI/CD pipeline
- Docker image build
- Amazon ECR image publishing
- ECS deployment automation
- GitHub Actions workflow

## Project Structure

```text
.github/workflows/
app/
docker/
diagrams/
screenshots/
```

## Key Learnings

- GitHub Actions workflows
- Container image lifecycle
- Amazon ECR integration
- Amazon ECS deployments
- CI/CD automation

## Status

✅ Completed

## Future Improvements

- Add automated testing
- Add Terraform provisioning
- Blue/Green deployments
- Security scanning with Trivy

