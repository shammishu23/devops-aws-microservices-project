Devops Project: Microservices Deployment on AWS

Overview:
This project demonstrates deploying a microservices-based application on
AWS using infrastructure as Code and containerization tools.

Tech Stack:
• AWS(EC2)
• Terraform(IaC)
• Docker
• Docker Compose

What I Implemented:
• Provisioned EC2 infrastructure using Terraform
• configured security groups and SSH access
• Installed Docker and managed containers
• Deployed a microservices voting application
• Exposed services via public IP (ports 8080 & 8081)

Architecture:
Terraform --> AWS EC2
        ↓
Docker
        ↓
Docker Compose
        ↓
Microservices App (Vote, Result, Redis, Worker, DB)

Challenges & Solutions:
• Fixed AMI issues in Terraform
• Resolved Docker Permission errors
• Handled port conflicts (8080 already in use)
• Fixed container build issues(Buildx problem)

Future Improvements:
• CI/CD pipeline using GitHub Actions
• Kubernetes deployment
• Automated infrastructure provisionig

