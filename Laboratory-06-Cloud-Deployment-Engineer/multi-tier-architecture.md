# Two-Tier Architecture

## Web/Application Tier

The Web/Application Tier is the part of the system that users access through a web browser. In this laboratory activity, Nextcloud serves as the web application. It provides the interface where users can access the application.

## Database Tier

The Database Tier stores and manages the application's data. In this activity, MariaDB is used as the database service. The Nextcloud application connects to MariaDB to access the information it needs.

## Why Separate Them?

Separating the application and database into different services helps organize the system and makes each service easier to manage. It also allows the application and database to be configured and maintained independently. Docker Compose helps coordinate these services so they can work together.
