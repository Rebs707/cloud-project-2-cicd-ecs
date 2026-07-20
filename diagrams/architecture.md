# Architecture

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
