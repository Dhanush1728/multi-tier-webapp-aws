📦 Multi-Tier Web Application (AWS + CI/CD)
🚀 Live Demo

🔗 https://d32chaxxcetx4.cloudfront.net

🔗 http://multi-tier-alb-1079659786.eu-north-1.elb.amazonaws.com

📌 Project Overview

Multi-Tier Web Application is a cloud-deployed full-stack web application built using AWS infrastructure and automated CI/CD deployment.

The application demonstrates real-world 3-tier architecture:

🌐 Frontend hosted on Amazon S3 + CloudFront

🖥 Backend running on Amazon EC2 (Node.js + Express)

🗄 Database using Amazon RDS (MySQL)

⚙ Automated CI/CD using GitHub Actions

This project showcases cloud architecture design, deployment automation, and backend-database integration.

✨ Features

Add users to database

Fetch users from RDS

Frontend connected to backend via ALB

Backend connected securely to RDS

CI/CD auto-deploy on every push to main

Load balancer health checks

Public CloudFront distribution

🏗 Architecture
User (Browser)
        ↓
CloudFront (CDN)
        ↓
Amazon S3 (Frontend)
        ↓
Application Load Balancer
        ↓
Amazon EC2 (Node.js Backend)
        ↓
Amazon RDS (MySQL Database)
🛠 Tech Stack
Layer	Technology
Frontend	HTML, CSS, JavaScript
Backend	Node.js, Express
Database	Amazon RDS (MySQL)
Hosting	Amazon EC2
Load Balancer	AWS Application Load Balancer
CDN	Amazon CloudFront
CI/CD	GitHub Actions
Cloud Platform	AWS
🔁 CI/CD Workflow

Code pushed to main branch

GitHub Actions automatically triggers

Workflow connects to EC2 via SSH

Backend code updated

Node.js server restarted automatically

This ensures continuous deployment without manual SSH login.

⚙ Environment Configuration

Environment variables used:

DB_HOST=multi-tier-db.cxo662iosvk3.eu-north-1.rds.amazonaws.com
DB_USER=admin
DB_PASSWORD=****
DB_NAME=myapp

Secrets are not committed to GitHub.

☁ Deployment Overview

High-level deployment steps:

Launch EC2 instance (Amazon Linux 2023)

Configure security groups

Set up RDS MySQL instance

Configure Application Load Balancer

Deploy frontend to S3

Configure CloudFront distribution

Implement GitHub Actions CI/CD pipeline

🔒 Security Practices

RDS not publicly accessible

Security groups restrict DB access to EC2 only

Secrets stored using environment variables

CI/CD SSH authentication via GitHub Secrets

Load Balancer health checks configured

📈 Future Improvements

HTTPS via ACM certificate

Docker containerization

Frontend CI/CD automation

Auto-scaling group

Monitoring using CloudWatch

🎓 Internship Project Highlights

This project demonstrates:

3-tier AWS architecture

Cloud deployment practices

Load balancing concepts

RDS integration

CI/CD automation

Secure networking configuration

👨‍💻 Author

Dhanush S
B.E Computer Science Engineering
Cloud & DevOps Enthusiast
