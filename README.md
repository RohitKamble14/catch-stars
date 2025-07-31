# 🎮 Catch the Stars – Game Deployment on AWS with ECS Fargate

A fast-paced browser game deployed using a modern CI/CD pipeline with **GitHub Actions**, **Amazon ECR**, and **ECS Fargate**. This project demonstrates hands-on experience in containerization, automation, and cloud-native deployment on AWS.

---

## 📸 Project Preview

![Catch the Stars Game Screenshot](https://github.com/RohitKamble14/catch-stars/blob/master/screenshots/Live-game.gif)

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
- Building Docker images with GitHub Actions
- Pushing images to ECR and deploying on ECS Fargate
- Managing AWS IAM roles, networking, and log monitoring

---

## 📄 License

[MIT](LICENSE)

---
