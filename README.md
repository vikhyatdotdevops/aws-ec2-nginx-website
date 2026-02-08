# AWS EC2 Web Deployment – DevOps Project

## Project Overview
This project demonstrates deploying a static website on AWS EC2 and progressively improving the deployment using DevOps practices.
The project includes manual deployment, CI/CD automation, Docker containerization, and Infrastructure as Code using Terraform.

The server runs on Amazon Linux 2023 and the website is accessible via the EC2 public IP.

---

## Tools & Technologies
- AWS EC2
- Amazon Linux 2023
- Nginx
- Docker
- Git & GitHub
- GitHub Actions
- Terraform
- Linux
- AWS Security Groups

---

## Phase 1: Manual Deployment (EC2 + Nginx)
- Launched EC2 instance using Amazon Linux 2023
- Configured Security Group for SSH (22) and HTTP (80)
- Connected to the instance using SSH
- Installed and configured Nginx
- Deployed a static HTML website
- Accessed the website using the EC2 public IP

---

## Phase 2: CI/CD Pipeline (GitHub Actions)
- Created CI/CD pipeline triggered on push to the main branch
- Configured GitHub Secrets for secure SSH authentication
- Automated deployment to AWS EC2 using GitHub Actions
- Eliminated the need for manual SSH-based deployments

---

## Phase 3: Dockerized Deployment
- Installed Docker on Amazon Linux 2023
- Created a Dockerfile using Nginx as the base image
- Built a custom Docker image for the website
- Deployed the website inside a Docker container
- Exposed container on port 80
- Resolved port conflicts by stopping host Nginx
- Verified application using browser and curl

---

## Phase 4: Infrastructure as Code (Terraform)

In this phase, AWS infrastructure was provisioned using Terraform instead of manual AWS Console steps.

### What was done
- Created AWS EC2 instance using Terraform
- Created Security Group allowing SSH (22) and HTTP (80)
- Used variables for reusable configuration
- Used outputs to display EC2 public IP
- Verified infrastructure by installing Nginx and accessing it via browser
- Destroyed infrastructure after use to avoid unnecessary AWS cost

### Terraform Commands Used
bash
terraform init
terraform plan
terraform apply
terraform destroy




