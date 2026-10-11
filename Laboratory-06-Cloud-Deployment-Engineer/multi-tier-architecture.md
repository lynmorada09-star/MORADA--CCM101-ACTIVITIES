Multi-Tier Architecture

What Is Two-Tier Architecture?

A two-tier architecture is an application design that separates an application into two main parts: the web/application tier and the database tier. These two tiers communicate with each other to provide the required services to users.

The Web/Application Tier

The web/application tier handles user requests and provides the application's user interface. In this laboratory activity, Nextcloud serves as the web application where users can access and manage their cloud files through a browser.

The Database Tier

The database tier stores and manages persistent information needed by the application. In this activity, MariaDB is used to store database information, including user account information and file metadata.

Why Separate Them?

Separating the web application and database into different containers makes the system easier to manage, update, and troubleshoot. Each service can be configured independently, and the application can be scaled without combining everything into a single container. This separation also helps organize the deployment.

Conclusion

The Nextcloud and MariaDB containers demonstrate how two services work together in a two-tier application architecture using Docker Compose.
