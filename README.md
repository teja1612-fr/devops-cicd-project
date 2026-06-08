 DevOps CI/CD Project

## What This Does

Automates the complete application deployment process using Jenkins, Docker, Kubernetes, SonarQube, and Nexus. The pipeline builds, tests, analyzes, packages, and deploys the application with minimal manual intervention.

## Tech Stack

Jenkins • Maven • SonarQube • Nexus • Docker • Kubernetes • GitHub • Linux

## How It Works

1. Code is pushed to GitHub.
2. Jenkins pipeline is triggered automatically.
3. Maven builds the application and runs tests.
4. SonarQube performs code quality analysis.
5. Build artifacts are stored in Nexus Repository.
6. Docker creates a container image for the application.
7. The image is deployed to Kubernetes using deployment manifests.
8. Application updates are delivered through an automated CI/CD workflow.

## Files

* `Jenkinsfile` – CI/CD pipeline definition.
* `Dockerfile` – Application container configuration.
* `pom.xml` – Maven build configuration.
* `deploymentfiles/` – Kubernetes deployment manifests.
* `src/` – Application source code.
* `target/` – Generated build artifacts.

## Key Concepts Demonstrated

* End-to-End CI/CD Pipeline
* Continuous Integration & Continuous Deployment
* Code Quality Analysis with SonarQube
* Artifact Management using Nexus
* Containerization with Docker
* Kubernetes Application Deployment
* DevOps Automation and Release Management
