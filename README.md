# Joy Akinleye — Cloud & DevOps Portfolio

A responsive personal portfolio built with HTML, CSS and vanilla JavaScript, containerised with Docker and deployed to AWS EC2 using GitHub Actions CI/CD.

## Live Portfolio

**Website:** http://13.51.194.212

**GitHub:** https://github.com/Bbyjayyy/joy-devops-portfolio

**LinkedIn:** https://www.linkedin.com/in/joy-akinleye

## Project Structure

```text
joy-devops-portfolio/
├── .github/
│   └── workflows/
│       └── deploy.yml
├── assets/
│   └── Joy_Oluwafunmiso_Akinleye_DevOps_CV.pdf
├── .dockerignore
├── .gitignore
├── Dockerfile
├── index.html
├── styles.css
├── script.js
└── README.md
```

## Technologies Used

- HTML5
- CSS3
- JavaScript
- Linux / Ubuntu
- Git and GitHub
- Docker
- AWS EC2
- GitHub Actions
- Nginx
- SSH

## Run Locally

Clone the repository:

```bash
git clone https://github.com/Bbyjayyy/joy-devops-portfolio.git
cd joy-devops-portfolio
```

Build the Docker image:

```bash
docker build -t joy-portfolio:latest .
```

Run the container:

```bash
docker run -d -p 8080:80 --name joy-portfolio-web joy-portfolio:latest
```

Open the website at:

```text
http://localhost:8080
```

## Deployment and CI/CD

The portfolio is deployed to an AWS EC2 Ubuntu instance and served through an Nginx Docker container.

GitHub Actions automates the deployment whenever changes are pushed to the `main` branch.

The workflow performs the following steps:

1. Checks out the repository.
2. Validates the required project files.
3. Builds the Docker image.
4. Connects securely to the EC2 instance using GitHub repository secrets and SSH host-key verification.
5. Pulls the latest code and rebuilds the Docker image on EC2.
6. Replaces the running container with the updated version.
7. Runs an HTTP health check to confirm that the website is responding.

## Projects

### 1. Linux Server Health Monitoring Script

A Bash scripting project developed on Ubuntu to check basic server health information, including disk usage, memory usage and running processes.

### 2. AWS Services Architecture Exercise

A conceptual cloud architecture exercise exploring AWS services for compute, networking, storage, security, monitoring and CI/CD.

## CV

My downloadable CV is available on the portfolio website.

## Project Status

The portfolio is deployed and accessible through its public EC2 address. Docker containerisation and automated GitHub Actions deployment have been implemented.