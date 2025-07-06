# 🚀 AWS DevOps CI/CD Pipeline Project (2025)
# aws-ci-cd-project

A complete hands-on AWS DevOps project showcasing a CI/CD pipeline using Git, Jenkins, Maven, Docker, and DockerHub. This project demonstrates automated code build, packaging, containerization, and deployment using AWS EC2 instances.

---

## 📌 Project Overview

**Goal**: Automate the build, test, and deployment of a Java-based web application using Jenkins and Docker, hosted on EC2.

**Architecture**:
- Dev system (Developer Machine)
- Jenkins server
- Docker Build System
- Docker Deploy Server

---

## 🔧 Tools & Technologies

- **AWS EC2** (Amazon Linux 2023)
- **Git & GitHub**
- **Jenkins**
- **Apache Maven**
- **Docker**

---

## 🧱 Project Structure

```bash
/myproject
├── Dockerfile
├── pom.xml
├── README.md
├── webapp/
│   ├── pom.xml
│   ├── src/
│   └── target/
│       └── webapp.war
└── server/
🔄 CI/CD Pipeline Steps
1️⃣ PullMyCode
Triggered manually or via Git polling.

Clones code from GitHub into /myproject.

2️⃣ BuildMyCode
Uses Maven to build and package the WAR file.

3️⃣ TransferMyCode
Sends webapp.war and Dockerfile via SSH to Docker Build Server.

4️⃣ PushCodeToDockerHub
Jenkins remotely builds Docker image and pushes it to Docker Hub.

5️⃣ DeployMyCode
Pulls image on Deploy Server and runs a container exposing port 8080.

📂 Docker Hub
Docker Image:
➡️ https://hub.docker.com/repository/docker/surajcloud/cloudproject

🌐 Application Access
Once the pipeline completes, visit:

Copy
Edit
http://<Deploy-Server-Public-IP>:8080
To view the running Java web app.

🙋‍♂️ Author
Suraj Karle
Aspiring Cloud/DevOps Engineer
