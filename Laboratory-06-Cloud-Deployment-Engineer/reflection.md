Mission Reflection

My Experience in Mission 6

In this laboratory activity, I learned how Docker Compose can simplify the deployment of a multi-tier application. Instead of starting the Nextcloud application and MariaDB database separately, I was able to define both services in a single YAML configuration file. This helped me understand how Infrastructure as Code makes deployment more organized and repeatable.

I also learned that YAML indentation is important. Incorrect spacing or the use of tabs instead of spaces can cause configuration errors. These errors may prevent Docker Compose from reading the file correctly, so checking the structure before deployment is necessary.

Environment variables were another important concept in this activity. Variables such as MYSQL_DATABASE, MYSQL_USER, and MYSQL_PASSWORD provide configuration values to the application and database containers. The MYSQL_HOST variable helps Nextcloud identify the database service. I also realized that passwords must be handled carefully, especially when preparing applications for real-world use.

Deploying Nextcloud helped me connect the concepts I learned in class with a practical cloud environment. I could see how an application and its database communicate through separate containers. Checking the container status and opening port 8080 also helped me understand the steps involved in making an application accessible through a browser.

Compared with Mission 1, my understanding of cloud computing has developed from learning basic concepts to practicing application deployment and infrastructure management. I now understand that cloud engineering involves not only running applications but also configuring, testing, documenting, and managing the resources they depend on.

Overall, this mission helped me appreciate the importance of automation, accurate configuration, and technical documentation. It also encouraged me to continue improving my skills in Linux, Docker, and cloud deployment.



