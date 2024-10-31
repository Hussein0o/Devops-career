# Full-Stack Application Deployment with Jenkins and Kubernetes

This project is a full-stack web application consisting of a **Flask** backend, a **MySQL** database, and a **HTML/CSS/JavaScript** frontend. It also includes configurations for **CI/CD** using **Jenkins** and **Kubernetes** deployments for scalability and orchestration. The purpose of this project is to demonstrate how to deploy and manage a multi-tier application using industry-standard DevOps practices.

## Table of Contents

- [Project Overview](#project-overview)
- [Folder Structure](#folder-structure)
- [Prerequisites](#prerequisites)
- [Installation and Setup](#installation-and-setup)
- [Running the Application](#running-the-application)
- [CI/CD Pipeline with Jenkins](#cicd-pipeline-with-jenkins)
- [Kubernetes Deployment](#kubernetes-deployment)
- [Contributing](#contributing)

## Project Overview

This project implements a three-tier web application with the following components:

1. **Backend (Flask)**: Handles the API logic and communicates with the MySQL database.
2. **Database (MySQL)**: Stores application data.
3. **Frontend (HTML/CSS/JavaScript)**: Provides a user interface for interaction.
4. **Jenkins CI/CD**: Automates the build, test, and deployment process.
5. **Kubernetes (KinD)**: Manages deployment, scaling, and networking.

## Folder Structure

├── backend-flask # Flask application code for the backend 
├── database-mysql # MySQL database configuration and schema
├── frontend-html # Static frontend files (HTML, CSS, JavaScript)
├── jenkins-tools # Jenkins configuration files and tools 
├── k8s-manifests # Kubernetes deployment files
├── kind-cluster.yml # KinD cluster setup configuration 
├── jenkinsfile # Jenkins pipeline definition 
└── README.md # Project overview and setup instructions

### File Descriptions

- **backend-flask**: Contains all backend code, endpoints, and Flask configurations.
- **database-mysql**: Includes SQL scripts and MySQL configurations.
- **frontend-html**: Houses static frontend assets (HTML, CSS, JS).
- **jenkins-tools**: Contains Jenkins-specific tools, plugins, and Docker files.
- **k8s-manifests**: Kubernetes deployment and service manifests.
- **kind-cluster.yml**: Configuration for deploying the application using KinD (Kubernetes in Docker).
- **jenkinsfile**: Defines the CI/CD pipeline steps for Jenkins.

## Prerequisites

- **Docker** and **Docker Compose**: For containerized development.
- **Jenkins**: To manage CI/CD pipelines.
- **Kubernetes**: Installed or configured using KinD (for local development).
- **Python 3.x**: To run the Flask backend locally.
- **Node.js and npm** (optional): If the frontend involves additional JavaScript libraries.

## Installation and Setup

### Step 1: Set Up the Database

Navigate to `database-mysql` and load the schema into MySQL:

```bash
mysql -u root -p < schema.sql

### File Descriptions

- **backend-flask**: Contains all backend code, endpoints, and Flask configurations.
- **database-mysql**: Includes SQL scripts and MySQL configurations.
- **frontend-html**: Houses static frontend assets (HTML, CSS, JS).
- **jenkins-tools**: Contains Jenkins-specific tools, plugins, and Docker files.
- **k8s-manifests**: Kubernetes deployment and service manifests.
- **kind-cluster.yml**: Configuration for deploying the application using KinD (Kubernetes in Docker).
- **jenkinsfile**: Defines the CI/CD pipeline steps for Jenkins.

## Prerequisites

- **Docker** and **Docker Compose**: For containerized development.
- **Jenkins**: To manage CI/CD pipelines.
- **Kubernetes**: Installed or configured using KinD (for local development).
- **Python 3.x**: To run the Flask backend locally.
- **Node.js and npm** (optional): If the frontend involves additional JavaScript libraries.

## Installation and Setup

### Step 1: Set Up the Database

Navigate to `database-mysql` and load the schema into MySQL:

```bash
mysql -u root -p < schema.sql
Kubernetes Deployment

Deployments are managed in k8s-manifests and include:
Contributing

Contributions are welcome! Please fork the repository and submit a pull request.


    Deployments: For backend, frontend, and database services.
    Services: Expose services within the cluster.
    Ingress (optional): Route external traffic to the frontend.
