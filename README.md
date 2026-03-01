# 📦 Multi-Tier Web Application (AWS + CI/CD)

## 🚀 Live Demo
- Frontend (CloudFront): https://d326chaxcctex4.cloudfront.net/
- Backend (ALB): http://multi-tier-alb-1079659786.eu-north-1.elb.amazonaws.com  

---

## 📌 Project Overview

This project is a cloud-deployed **3-tier web application** built using AWS services and automated using a CI/CD pipeline.

The application follows a real-world architecture:
- Frontend hosted on **Amazon S3 + CloudFront**
- Backend deployed on **Amazon EC2 (Node.js + Express)**
- Database managed using **Amazon RDS (MySQL)**
- Automated deployment using **GitHub Actions (CI/CD)**

---

## ✨ Features

- Add user data through frontend
- Fetch user data from RDS database
- Load-balanced backend using ALB
- Secure database access via security groups
- Automatic backend deployment on every GitHub push
- Health checks via Application Load Balancer

---

## 🏗 Architecture

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

---

## 🛠 Tech Stack

| Layer | Technology |
|------|------------|
| Frontend | HTML, CSS, JavaScript |
| Backend | Node.js, Express |
| Database | Amazon RDS (MySQL) |
| Hosting | Amazon EC2 |
| Load Balancer | AWS Application Load Balancer |
| CDN | Amazon CloudFront |
| CI/CD | GitHub Actions |
| Cloud Platform | AWS |

---

## 🔁 CI/CD Workflow

1. Code is pushed to the `main` branch
2. GitHub Actions pipeline is triggered
3. Workflow connects to EC2 via SSH
4. Backend code is pulled and dependencies installed
5. Node.js server is restarted automatically

This ensures **continuous deployment without manual intervention**.

---

## ⚙ Environment Variables

Sensitive configuration is handled using environment variables:

```
DB_HOST=multi-tier-db.cxo662iosvk3.eu-north-1.rds.amazonaws.com
DB_USER=admin
DB_PASSWORD=********
DB_NAME=myapp
```

Secrets are not committed to the repository.

---

## ☁ Deployment Overview

High-level deployment steps:
1. Launch EC2 instance (Amazon Linux 2023)
2. Create RDS MySQL database
3. Configure security groups
4. Set up Application Load Balancer
5. Host frontend on S3
6. Enable CloudFront distribution
7. Configure GitHub Actions CI/CD pipeline

---

## 🔒 Security Practices

- RDS database is not publicly accessible
- Database access restricted to EC2 security group
- Secrets stored as environment variables
- SSH authentication via GitHub Secrets
- Load balancer health checks enabled

---

## 📈 Future Improvements

- HTTPS using ACM certificate
- Docker containerization
- Frontend CI/CD automation
- Auto Scaling Group for backend
- Monitoring using CloudWatch

---

## 🎓 Internship Project Highlights

This project demonstrates:
- 3-tier AWS architecture
- Cloud deployment practices
- Load balancing concepts
- Database integration
- CI/CD automation using GitHub Actions
- Secure cloud networking

---

## 👨‍💻 Author

**Dhanush S**  
B.E Computer Science Engineering  
Cloud & DevOps Enthusiast
