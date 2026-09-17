# Mission 4 Reflection

This laboratory helped me understand why containers are useful compared to traditional virtual machines. A Docker container can start much faster because it does not need to install and run a complete guest operating system like a virtual machine. In my experience, Docker only needed a few commands before I could run the Nginx application.

The port mapping `-p 8080:80` is important because it connects port 8080 on the host to port 80 inside the Nginx container. This allows me to access the web server using the host machine's port. Without the port mapping, the Nginx service inside the container would not be directly accessible through that host port.

I also learned what happens when a container is removed using `docker rm`. The container itself is deleted, so information stored only inside that container can be lost. This showed me why persistent storage is important when an application needs to keep data even after a container is removed.

Containerization can also improve teamwork between developers and IT operations. Developers can package an application with its required environment, while the operations team can run the same container using Docker. This can make deployment more consistent and easier to manage.

After completing this mission, my GitHub portfolio has become more useful because it now contains another hands-on cloud computing activity. I was able to document Docker commands, deploy Nginx, and manage a container. This experience helped me better understand how cloud-native applications can be developed and operated.
