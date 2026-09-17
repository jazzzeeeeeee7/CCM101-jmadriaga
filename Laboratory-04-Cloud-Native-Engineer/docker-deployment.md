# Docker Deployment

## Container Lifecycle

### 1. List Running Containers

Command:
docker ps

This command lists the Docker containers that are currently running.

### 2. Stop the Running Container

Command:
docker stop nginx-server

This command stops the running Nginx container.

### 3. Verify It Is Stopped

Command:
docker ps -a

This command displays all containers and allows me to verify that the Nginx container has stopped.

### 4. Remove the Container Completely

Command:
docker rm nginx-server

This command completely removes the stopped Nginx container from the Docker environment.

## Screenshot

The terminal execution of the container lifecycle commands was captured and saved as:

container-lifecycle.png
