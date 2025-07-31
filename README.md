# 🎮 Catch the Stars – Game Deployment on AWS with ECS Fargate

A fast-paced browser game deployed via a modern CI/CD pipeline using **GitHub Actions**, **Amazon ECR**, and **ECS Fargate**. This project showcases hands-on experience in containerization, automation, and cloud-native deployment using AWS services.

---

## 🚀 Live Demo

🕹️ Hosted via ECS Fargate  
**[Replace this with your actual IP address or domain name]**

---

## 📸 Project Preview

<img src="https://user-images.githubusercontent.com/your-image-path/catch-the-stars-preview.png" alt="Catch the Stars Game Screenshot" style="max-width:100%;" />

<!--  
Replace the src above with the actual image path if hosted in the repo or use a relative path like:
<img src="assets/catch-the-stars-preview.png" alt="Catch the Stars Game Screenshot" style="max-width:100%;" />
-->

---

## 🔧 Tech Stack

| Component         | Tool/Service                      |
|-------------------|-----------------------------------|
| Frontend Game     | HTML, CSS, JavaScript             |
| Backend Server    | Node.js, Express.js               |
| Containerization  | Docker                            |
| CI/CD Pipeline    | GitHub Actions                    |
| Image Registry    | Amazon Elastic Container Registry |
| Deployment        | Amazon ECS (Fargate)              |
| Logging           | Amazon CloudWatch                 |

---

## 🧠 Project Architecture

```mermaid
graph TD
    A[Local Project Code (GitHub)] --> B[GitHub Actions (CI/CD)]
    B --> C[Docker Image Built & Pushed to ECR]
    C --> D[Manual ECS Fargate Deployment (AWS Console)]
    D --> E[Game Publicly Accessible in the Cloud]
```

---

## 📁 Folder Structure

```
catch-stars/
├── public/
│   └── index.html      # Game code (HTML/CSS/JS)
├── server.js           # Express server
├── package.json        # Dependencies
├── Dockerfile          # Build instructions
└── .github/
    └── workflows/
        └── deploy.yml  # GitHub Actions workflow
```

---

## ⚙️ GitHub Actions Workflow

Automated CI/CD pipeline builds and pushes Docker images to Amazon ECR on every push to `main`.

```yaml
on:
  push:
    branches: [ main ]
jobs:
  build-and-deploy:
    runs-on: ubuntu-latest
    steps:
      - name: Build and Push to ECR
        # Build Docker image and push to Amazon ECR
        # (See full file in .github/workflows/deploy.yml)
```

---

## 📌 AWS Services Used

- **Amazon ECS Fargate** – Serverless container hosting
- **Amazon ECR** – Docker image storage
- **CloudWatch Logs** – Real-time log monitoring
- **IAM Roles** – Secure access for GitHub Actions and ECS
- **VPC & Subnets** – Secure and scalable networking

---

## 💡 What I Learned

- Serving a static game via Node.js & Express
- Writing a production-ready Dockerfile
- Building Docker images with GitHub Actions (not locally!)
- Pushing images to ECR and deploying on ECS Fargate
- Managing AWS IAM roles, networking, and log monitoring

---

## 📝 How to Deploy

1. **Clone this repository**
2. **Set up AWS credentials** in your GitHub repo secrets (`AWS_ACCESS_KEY_ID`, `AWS_SECRET_ACCESS_KEY`, `AWS_REGION`, etc.)
3. **Configure ECR repository** and update the workflow with your ECR details.
4. **Push to `main` branch** to trigger CI/CD.
5. **Deploy the latest image to ECS Fargate** via AWS Console or CLI.
6. **Access your game** at your Fargate service's public endpoint.

---
