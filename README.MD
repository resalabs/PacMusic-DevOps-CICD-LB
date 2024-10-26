# PacMusic

PacMusic is a simple web-based music streaming application that allows users to browse and play music from a curated list. This project serves as a demonstration of a full CI/CD pipeline setup using GitHub Actions, Docker, and automated deployments.

## Project Overview

The repository includes:
- A basic web application built with Python and Flask.
- Docker setup for containerization and easy deployment.
- GitHub Actions workflows for CI/CD:
  - **Dev Testing**: Runs automated tests on pull requests to the `main` branch.
  - **Staging Deployment**: Automatically deploys updates to the staging server on each push to the `main` branch.
  - **Production Deployment**: Deploys the application to production upon release creation.
  - **Container Registry**: Builds and pushes Docker images to a private Docker Hub repository.

## Key Features

- **Music Streaming**: Users can play music from a list on the `/` route.
- **Automated CI/CD**: Integration of GitHub Actions for continuous integration and deployment.
- **Dockerized Application**: Dockerized for consistent environment management across development, staging, and production.

## Technology Stack

- **Python & Flask**: Backend framework for the web application.
- **Docker**: Containerization for consistent deployments.
- **GitHub Actions**: Automation of testing, building, and deployment processes.
- **MinIO**: Object storage for managing media files (configured through environment variables).

## Getting Started

To clone and run the project locally:

```bash
git clone https://github.com/hudiyaresa/PacMusic-DevOps-CICD.git
cd pacmusic
docker-compose up --build
```

Make sure to configure environment variables as needed in a `.env` file for local development.

