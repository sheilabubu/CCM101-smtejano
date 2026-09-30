# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

In this laboratory, I deployed a multi-tier private cloud storage application using Docker Compose. The application used Nextcloud as the web application and MariaDB as the database. Instead of deploying the containers separately, I used a `docker-compose.yml` file to define and deploy the entire stack.

## Objectives

* Understand the concept of multi-tier application architecture.
* Create a Docker Compose configuration file.
* Deploy Nextcloud and MariaDB as multiple containers.
* Use Docker Compose to manage the application stack.
* Access the Nextcloud web interface through port 8080.
* Document the deployment process using Markdown.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```

## Skills Learned

* Creating and editing YAML configuration files.
* Using Docker Compose to deploy multiple containers.
* Understanding the roles of an application container and a database container.
* Connecting containers using Docker Compose service names.
* Using environment variables to configure container applications.
* Checking container status and shutting down a multi-container application.
* Documenting cloud deployment procedures using Markdown.
