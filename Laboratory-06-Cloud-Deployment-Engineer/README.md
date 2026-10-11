Mission 6: The Cloud Deployment Engineer

Mission Overview

This laboratory activity demonstrates how to deploy a multi-tier cloud storage application using Docker Compose. The application consists of Nextcloud as the web application and MariaDB as the database.

Objectives

- Understand two-tier application architecture.
- Create a Docker Compose YAML configuration file.
- Deploy Nextcloud and MariaDB containers.
- Access the Nextcloud web interface through port 8080.
- Document the deployment using Markdown.
- Practice Infrastructure as Code principles.

Commands Executed

mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down

Skills Learned

- Linux terminal navigation and file management.
- Editing YAML files using Nano.
- Configuring Docker Compose services.
- Deploying and stopping multiple containers.
- Understanding application-to-database communication.
- Documenting cloud deployment procedures using Markdown.
