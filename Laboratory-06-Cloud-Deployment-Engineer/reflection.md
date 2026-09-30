# Mission 6 Reflection

Writing a `docker-compose.yml` file makes a cloud engineer's job easier because multiple containers can be defined in one configuration file. Instead of manually creating and configuring each container separately, Docker Compose can deploy the related services together. This makes the deployment process more organized and repeatable.

YAML indentation is very important because YAML uses spaces to define the structure of the configuration. If I accidentally use a Tab or incorrect indentation, Docker Compose may not understand the file correctly and the deployment can fail. This showed me that even small formatting errors can affect an infrastructure configuration.

We used environment variables such as `MYSQL_PASSWORD` to provide the configuration values needed by the containers. These variables allow the Nextcloud application and MariaDB database to communicate using the required settings.

It was interesting to see how a complete cloud storage application could be deployed within a few minutes. Using Docker Compose made the process much simpler because Nextcloud and MariaDB could be deployed as connected services instead of being configured completely separately.

Since Mission 1, my understanding of Cloud Computing has developed from learning basic cloud concepts and Linux commands to working with containers and Infrastructure as Code. I now understand that cloud engineers can automate infrastructure deployment using configuration files. This mission also helped me understand how different application components can work together as a multi-tier system.

