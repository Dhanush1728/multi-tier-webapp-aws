# Multi-Tier Web Application with CI/CD (AWS)

## Objective
Deploy a 3-tier web application (Frontend, Backend, Database) with a CI/CD pipeline using AWS and GitHub Actions.

## Architecture
Frontend → S3 + CloudFront  
Backend → EC2 (Node.js + Express)  
Database → Amazon RDS (MySQL)  
CI/CD → GitHub Actions (Auto deploy to EC2)

## Tech Stack
- Frontend: HTML, CSS, JavaScript
- Backend: Node.js, Express
- Database: MySQL (Amazon RDS)
- Cloud: AWS EC2, S3, CloudFront, ALB
- CI/CD: GitHub Actions

## CI/CD Workflow
- Code pushed to `main` branch
- GitHub Actions runs automatically
- Backend is deployed to EC2 using SSH
- Node.js server restarts after deployment

## Live URLs
- Frontend (CloudFront): https://d326chaxcctex4.cloudfront.net
- Backend (via ALB): http://multi-tier-alb-1079659786.eu-north-1.elb.amazonaws.com

## Proof of Work
- GitHub Actions workflow runs successfully
- Backend connected to RDS
- Users can be added and fetched from database

## Author
Dhanush S  
Codec Technologies – Internship Project
