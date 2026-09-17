# Docker Deployment

## Nginx Deployment

First, I pulled the official Nginx image using:

docker pull nginx

This command downloads the Nginx image that will be used to create the container.

Next, I created and started the Nginx container using:

docker run -d -p 8080:80 --name nginx-server nginx

This command runs Nginx in the background and maps host port 8080 to container port 80.

To verify that the Nginx server was working, I used:

curl http://localhost:8080

This command checks if the Nginx web server can be accessed through port 8080.

## Container Lifecycle

### 1. List Running Containers

docker ps

This command lists the Docker containers that are currently running.

### 2. Stop the Running Container

docker stop nginx-server

This command stops the running Nginx container.

### 3. Verify It Is Stopped

docker ps -a

This command displays all containers and allows me to verify that the Nginx container has stopped.

### 4. Remove the Container Completely

docker rm nginx-server

This command completely removes the stopped Nginx container from the Docker environment.

## Summary

Through this activity, I learned how to pull a Docker image, run an Nginx container, use port mapping, check the container status, stop a container, and remove it from the Docker environment.
