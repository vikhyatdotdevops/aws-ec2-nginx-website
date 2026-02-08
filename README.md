# AWS EC2 Website Hosting using Nginx

## 📌 Project Overview
This project demonstrates hosting a static website on AWS EC2 using Nginx.
The server runs on Amazon Linux 2023 and is accessible via a public IP.

## 🛠 Services & Tools Used
- AWS EC2
- Amazon Linux 2023
- Nginx
- Security Groups
- Linux (SSH)

## 🚀 Steps Performed
1. Created an EC2 instance (t2.micro)
2. Configured Security Group to allow SSH (22) and HTTP (80)
3. Connected to the instance using SSH
4. Installed and configured Nginx
5. Deployed a custom HTML website
6. Accessed the website using Public IP

## 💻 Commands Used
```bash
sudo dnf update -y
sudo dnf install nginx -y
sudo systemctl start nginx
sudo systemctl enable nginx

## 🔁 CI/CD Pipeline
- Implemented automated deployment using GitHub Actions
- Used SSH-based deployment to AWS EC2
- Managed sensitive credentials using GitHub Secrets
- Achieved zero-touch deployment on every push to main branch
