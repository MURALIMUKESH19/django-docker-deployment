# Django Docker Deployment

This repository contains a Django application deployed with Docker. It integrates with a PostgreSQL database and is set up for continuous integration and deployment (CI/CD) using Jenkins.

## Project Setup

This project uses Docker and Docker Compose to containerize the Django application and PostgreSQL database. Jenkins is used for automating the build and deployment process.

### Technologies Used
- **Django**: A Python-based web framework for building web applications.
- **PostgreSQL**: A relational database management system.
- **Docker**: Containerization platform for packaging applications.
- **Docker Compose**: Tool for defining and running multi-container Docker applications.
- **Jenkins**: Open-source automation server used for continuous integration/continuous deployment (CI/CD).
  
## Prerequisites

Before you begin, ensure you have met the following requirements:

- **Docker**: [Install Docker](https://docs.docker.com/get-docker/) on your machine.
- **Docker Compose**: [Install Docker Compose](https://docs.docker.com/compose/install/).
- **Jenkins**: Follow the instructions to install Jenkins [here](https://www.jenkins.io/doc/book/installing/).

## Setup Instructions

### 1. Clone the Repository
Clone this repository to your local machine:
```bash
git clone https://github.com/MURALIMUKESH19/django-docker-deployment.git
cd django-docker-deployment

docker-compose up --build

docker exec jenkins cat /var/jenkins_home/secrets/initialAdminPassword

django-docker-deployment/
│
├── Dockerfile                   # Dockerfile for the Django application
├── docker-compose.yml           # Docker Compose configuration file
├── jenkins/
│   ├── Jenkinsfile              # Jenkins pipeline file
├── manage.py                   # Django management script
├── requirements.txt             # Python dependencies
└── README.md                    # This file

### How to add this to your repository:
1. Open a text editor (like Notepad or Visual Studio Code).
2. Paste the above content.
3. Save it as `README.md`.
4. Follow the steps to add, commit, and push it to your GitHub repository (as I mentioned earlier).

This `README.md` file will help you to explain the project setup and how to run the application, providing a clear understanding for users and collaborators. Let me know if you need more adjustments!
