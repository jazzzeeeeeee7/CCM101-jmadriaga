# Laboratory Activity 7: The Cloud Operations Engineer

## Mission Overview

This activity focused on checking the condition and performance of a Linux server and a Docker container. I used different commands to view system resources, launched an Nginx web server, tested website requests, and examined the logs and container statistics to understand how monitoring works.

## Objectives

- Examine the available memory and disk space of a Linux server.
- Observe running processes and CPU activity.
- Run an Nginx web server inside a Docker container.
- Test website access and produce an HTTP error.
- Inspect server requests through Docker logs.
- Check the resource consumption of the container.
- Organize and record the activity results in Markdown.

## Monitoring Commands Executed

| Command | Description |
|---|---|
| `free -h` | Viewed the server's RAM usage and available memory. |
| `df -h /` | Checked the storage capacity and remaining space of the root filesystem. |
| `top` | Observed active processes and CPU performance. |
| `docker run -d -p 8080:80 --name client-website nginx` | Started an Nginx container and connected its web service to port 8080. |
| `docker ps` | Verified the status of the running container. |
| `curl http://localhost:8080` | Sent requests to test whether the website could be accessed. |
| `curl http://localhost:8080/hidden-admin-page` | Requested a nonexistent page to produce a 404 response. |
| `docker logs client-website` | Examined the recorded website requests and error responses. |
| `docker stats` | Viewed the container's current CPU, memory, and network statistics. |

## Skills Learned

Through this activity, I gained more experience using Linux commands and managing a Docker-based web server. I learned to check system resources, test website connectivity, and examine logs to find errors. I also understood how monitoring container statistics helps identify possible performance issues. These skills are useful for checking server health and helping applications operate reliably.
