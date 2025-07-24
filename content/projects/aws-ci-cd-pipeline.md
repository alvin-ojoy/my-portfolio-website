---
title: "Automated CI/CD Pipeline with AWS & Terraform"
date: 2024-11-15
tags: ["devops", "aws", "terraform", "ci-cd"]
thumbnail: "/images/projects/aws-pipeline-thumbnail.jpg"
github_url: "https://github.com/yourusername/aws-terraform-cicd"
---

## Overview
A **serverless CI/CD pipeline** built on AWS (CodePipeline, ECS, Terraform) to deploy a containerized Python app with zero-downtime blue/green deployments.

![Architecture Diagram](/images/projects/aws-cicd-architecture.png)  
*Diagram: AWS services used (CodeCommit → CodeBuild → CodeDeploy → ECS)*

## Key Features
- ✅ **Infrastructure as Code**: Terraform-managed AWS resources (VPC, ECS, IAM roles)  
- 🔄 **Blue/Green Deployments**: Automated traffic shifting via AWS CodeDeploy  
- 🔐 **Security**: Secrets management with AWS Parameter Store + IAM least privilege  
- 📊 **Monitoring**: CloudWatch alarms for pipeline failures  

## Technical Stack
```plaintext
AWS Services:
- CodePipeline, CodeBuild, CodeDeploy
- ECS Fargate (serverless containers)
- Terraform (v1.5+)

Tools:
- Docker, GitHub Actions (for linting)
- Trivy (container vulnerability scanning)