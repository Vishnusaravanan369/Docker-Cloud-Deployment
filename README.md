# Cloud Deployment & DevOps Implementation (Docker, Git, AWS)

This project demonstrates containerizing front-end applications and deploying them on AWS EC2 instances using Docker and GitHub. The workflow includes building Docker images, managing containers, and troubleshooting deployment issues.

## Project Duration
**Apr 2025 - May 2025**

## Project Overview
- Containerized front-end applications (HTML/CSS/JS) using Docker to create lightweight, custom images.
- Cloned and configured GitHub repositories on AWS EC2 Ubuntu instances.
- Deployed static websites via Dockerized Nginx containers.
- Built and published Docker images to Docker Hub with proper versioning and tagging.
- Managed container lifecycles (`docker run`, `exec`, `stop`, `rm`) and optimized system resources with cleanup commands.
- Troubleshot deployment errors (e.g., 403 errors, port conflicts) by analyzing logs and refining Dockerfile instructions.
- Tested images on both Docker Desktop and remote Ubuntu instances to ensure consistency.

## Tools & Technologies
- Docker & Docker Hub
- GitHub
- AWS EC2 (Ubuntu)
- Nginx
- CLI (Command Line Interface)

## Steps to Deploy
1. Clone the repository:
```bash
git clone https://github.com/<your-username>/docker-cloud-deployment.git
2.Build Docker image:

docker build -t <image-name>:<tag> .

3.Run container:

docker run -d -p 80:80 <image-name>:<tag>

4.Verify deployment by visiting your EC2 instance public IP in the browser.

5.Push image to Docker Hub:

docker login
docker tag <image-name>:<tag> <dockerhub-username>/<image-name>:<tag>
docker push <dockerhub-username>/<image-name>:<tag>


   

