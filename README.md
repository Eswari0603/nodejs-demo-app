# nodejs-demo-app
This repository demonstrates a CI/CD pipeline using GitHub Actions to build and deploy a Node.js app as a Docker image to DockerHub.

#Features

Node.js application

Dockerized for container deployment

Automated CI/CD pipeline with GitHub Actions

Pushes Docker image to DockerHub on main branch

#Prerequisites

DockerHub account

GitHub repository

Node.js installed locally (for testing)

GitHub Actions secrets configured:

DOCKER_USERNAME → Your DockerHub username

DOCKER_PASSWORD → DockerHub access token with write/publish scope

#Usage
Clone the repository
git clone https://github.com/Eswari0603/nodejs-demo-app.git
cd nodejs-demo-app

Build locally (optional)
docker build -t eswari06/nodejs-demo-app:latest .

Run locally
docker run -p 3000:3000 eswari06/nodejs-demo-app:latest


#CI/CD Pipeline

Triggered on push to main branch

Steps in .github/workflows/main.yml:

1.Checkout code

2.Build Docker image

3.Login to DockerHub

4.Push Docker image to DockerHub

#DockerHub

Repository: https://hub.docker.com/repository/docker/eswari06/nodejs-demo-app

Image tag: latest
