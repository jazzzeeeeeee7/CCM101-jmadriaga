# Docker Deployment

## Nginx Container Deployment

For this activity, I used Docker to pull an Nginx image and run it as a container.

### Commands Used

`docker pull nginx`

This command downloaded the official Nginx image needed for the container.

`docker run -d -p 8080:80 --name nginx-server nginx`

This command created and started the Nginx container in the background while mapping host port 8080 to container port 80.

`curl http://localhost:8080`

This command checked whether the Nginx web server was accessible through port 8080 and displayed the Nginx welcome page.

## Container Lifecycle

`docker ps`

This command listed the Docker containers that were currently running.

`docker stop nginx-server`

This command stopped the running Nginx container.

`docker ps -a`

This command displayed all containers and allowed me to verify that the Nginx container was stopped.

`docker rm nginx-server`

This command completely removed the stopped Nginx container.

`docker ps -a`

This command was used again to confirm that the Nginx container had been removed from the Docker environment.
