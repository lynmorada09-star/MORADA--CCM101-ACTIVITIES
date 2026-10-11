Docker Compose Guide

1. What Does the "services:" Block Do?

The "services:" block defines the containers or services that Docker Compose will create and manage. In this activity, it defines the MariaDB database service and the Nextcloud application service.

2. How Does Nextcloud Find the Database?

The "MYSQL_HOST=database" environment variable tells the Nextcloud application which database host to connect to. The name "database" refers to the database service defined in the Docker Compose configuration.

3. Difference Between "docker run" and "docker-compose up -d"

The "docker run" command is used to start an individual container with specified options. The "docker-compose up -d" command reads the Compose configuration and starts the services defined in the file together in the background.

4. Infrastructure as Code (IaC)

Infrastructure as Code means defining infrastructure using configuration files instead of manually setting up every component. Docker Compose makes the deployment easier to repeat and manage using a single configuration file.
