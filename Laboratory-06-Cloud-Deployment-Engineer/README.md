Mission 6: The Cloud Deployment Engineer

Mission Overview

This laboratory activity demonstrates how to deploy a two-tier cloud storage application using Docker Compose. The application uses Nextcloud as the web application and MariaDB as the database.

Objectives

- Explain two-tier application architecture.
- Create a Docker Compose YAML configuration file.
- Deploy Nextcloud and MariaDB using Docker Compose.
- Access the Nextcloud setup page through port 8080.
- Document the deployment process using Markdown.
- Practice Infrastructure as Code principles.

Commands Executed

mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down

Skills Learned

- Linux terminal navigation and directory management.
- Creating and editing YAML configuration files.
- Deploying multiple containers with Docker Compose.
- Understanding communication between an application and a database.
- Accessing a containerized web application through a mapped port.
- Writing technical documentation in Markdown.
- Collecting screenshots as deployment evidence.
