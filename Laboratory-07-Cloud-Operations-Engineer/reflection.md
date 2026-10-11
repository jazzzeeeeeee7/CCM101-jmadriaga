# Mission 7 Reflection: The Cloud Operations Engineer

This laboratory activity helped me understand how to monitor a Linux server and a Docker container. I learned that checking the server's resources is important even when the application is running properly. If the server has limited memory or disk space, the application may become slow or stop working. Monitoring these resources helps prevent problems and keeps the server in good condition.

The `docker logs` command is also useful when a user experiences problems with a web application. It allows us to see the requests and errors recorded by the container. In this activity, I tested a page that did not exist and received a 404 error. By checking the logs, I could identify the failed request and understand what happened when the page was accessed.

I also learned that logs and metrics have different purposes. Logs contain records of events, such as website requests and errors. Metrics provide numerical information about performance, including CPU usage, memory consumption, and network activity. Using both helps an engineer understand application problems and check whether the container is using resources properly.

For companies that manage thousands of containers, monitoring tools such as Prometheus and Grafana can be helpful. Prometheus collects performance metrics, while Grafana presents information through dashboards and graphs. These tools make it easier for engineers to monitor many applications and identify possible issues.

Overall, this activity improved my knowledge of Linux commands and Docker monitoring. I learned to examine system resources, test a web server, read application logs, and check container performance. Instead of guessing when a problem occurs, I can use the information collected from logs and metrics to investigate the cause. These skills will help me understand cloud operations and troubleshoot technical problems more effectively.

