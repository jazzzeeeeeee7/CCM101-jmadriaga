# Docker Compose Guide

## What does the services: block do?

The `services:` block defines the containers that will be created and managed by Docker Compose. In this deployment, it contains two services: the `database` service for MariaDB and the `app` service for Nextcloud.

## How did the Nextcloud app container know how to find the database container?

The Nextcloud app container uses the `MYSQL_HOST` environment variable to find the database container. The value is set to `database`, which matches the name of the MariaDB service in the Docker Compose file.

## What is the difference between docker run and docker-compose up -d?

The `docker run` command is used to create and start a single Docker container. On the other hand, `docker-compose up -d` uses the `docker-compose.yml` configuration file to create and start multiple related containers together in the background.

