# Neel POC - ECS CI/CD Pipeline

This repo builds a Docker image with a custom HTML page using NGINX, pushes it to ECR, and automatically deploys it to ECS (EC2 launch type) using CodePipeline and CodeBuild.

## 🔁 Workflow
- Push code to this repo (e.g., GitHub or CodeCommit)
- CodePipeline runs
- CodeBuild builds and pushes image to ECR
- ECS service auto-updates with the new image

## 🔧 Config
- ECR: `200901485389.dkr.ecr.us-east-1.amazonaws.com/neel-poc-ecr`
- ECS Cluster: `your-cluster-name`
- ECS Service: `your-service-name`

