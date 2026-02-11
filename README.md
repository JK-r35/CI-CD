🚀 CI/CD Pipeline – Docker + GitHub Actions + EC2
📌 Project Overview

This project demonstrates a simple CI/CD pipeline that automatically deploys a static web page to an AWS EC2 instance using Docker and GitHub Actions.

 @ Whenever code is pushed to the main branch:

 @ GitHub Actions triggers automatically

 @ Docker image is built

 @ Application is deployed to EC2 via SSH

 @ Website updates automatically

🛠 Tech Stack

 @ Docker

 @ GitHub Actions

 @ AWS EC2

 @ Nginx
  
 @ Linux (Ubuntu)

⚙️ CI/CD Workflow

   @ Developer pushes code to GitHub

   @ GitHub Actions runs workflow

   @ Files copied to EC2

   @ Docker image built

   @ Old container removed

   @New container deployed

🌍 Architecture

Developer → GitHub → GitHub Actions → EC2 → Docker → Live Website


EC2 Setup (One-Time Setup)
1️⃣ Launch EC2

 1. Ubuntu instance

 2. Allow HTTP (port 80) in Security Group

 3. Allow SSH (port 22)

2️⃣ Install Docker in EC2

SSH into EC2:

      sudo apt update
      sudo apt install docker.io -y
      sudo systemctl start docker
      sudo systemctl enable docker
      sudo usermod -aG docker ubuntu





