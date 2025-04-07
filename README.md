# 🚀 Node.js CI/CD App

This is a simple Node.js app deployed using a CI/CD pipeline with GitHub Actions and Docker.  
The Hosting was done manually on an AWS EC2 instance using Docker. (Could have done Automation here by changine the main.yml file but chose manual to host application)

---

## ⚙️ Tech Stack

- **Node.js** – App runtime  
- **Express** – Web framework  
- **Docker** – Containerization  
- **GitHub Actions** – CI/CD pipeline  
- **AWS EC2** – Manual hosting environment

---

## 🛠 CI/CD Workflow (GitHub Actions)

1. Triggered on push to the `main` branch  
2. Install Node.js dependencies  
3. Build Docker image of the app  
4. Push Docker image to DockerHub  

> The CI/CD pipeline is defined in `.github/workflows/main.yml`.

---

## 📦 DockerHub

👉 [DockerHub (nodejs-demo-app)](https://hub.docker.com/u/adijawanjal)

---

## ☁️ Deployment

The application was **manually hosted** on an **AWS EC2 instance** using Docker.

### 🔧 Manual hosting Steps

1. **Launch an EC2 instance** (Ubuntu) via AWS Console

2. **SSH into the EC2 instance**:
   ```bash
   ssh ubuntu@<your-ec2-public-ip>
3. Login to Docker Registry and Pull Image
4. Create Container with Pulled Image
