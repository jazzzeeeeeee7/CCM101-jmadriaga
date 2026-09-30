# Laboratory 06 – Cloud Deployment Engineer

## Mission Overview

This laboratory focuses on deploying a multi-tier private cloud storage application using Docker Compose. The application uses Nextcloud as the web/application tier and MariaDB as the database tier. Docker Compose allows both containers to be deployed and managed together.

## Objectives

* Understand the concept of a multi-tier application architecture.
* Understand the purpose and structure of a `docker-compose.yml` file.
* Use the Linux `nano` text editor to create configuration files.
* Deploy a multi-container application using Docker Compose.
* Understand Infrastructure as Code (IaC) principles.
* Document the deployment procedures using Markdown.

## Commands Executed

| Command                      | Purpose                                                                    |
| ---------------------------- | -------------------------------------------------------------------------- |
| `mkdir nextcloud-deployment` | Creates a new directory for the Nextcloud deployment project.              |
| `cd nextcloud-deployment`    | Enters the project directory.                                              |
| `nano docker-compose.yml`    | Opens Nano to create and edit the Docker Compose configuration file.       |
| `ls`                         | Lists the files and folders in the current directory.                      |
| `cat docker-compose.yml`     | Displays the contents of the Docker Compose file.                          |
| `docker-compose up -d`       | Starts and deploys the Nextcloud and MariaDB containers in the background. |
| `docker-compose ps`          | Checks and displays the status of the containers.                          |
| `docker-compose down`        | Stops and removes the containers created by Docker Compose.                |

## Skills Learned

* Linux command-line operations
* Docker Compose
* YAML configuration
* Multi-tier application deployment
* Container management
* Infrastructure as Code (IaC)
* Technical documentation using Markdown

