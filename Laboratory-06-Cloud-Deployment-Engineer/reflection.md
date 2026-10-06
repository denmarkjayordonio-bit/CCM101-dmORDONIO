# Mission Reflection

This mission gave me a better understanding of how cloud applications can be deployed using containers. One thing I noticed was how much easier Docker Compose makes the work of a cloud engineer. Instead of typing separate commands for MariaDB and Nextcloud, I could put their configurations inside one `docker-compose.yml` file. Once the file was ready, one command was enough to start the whole setup.

I also learned that YAML files need to be written carefully. The indentation is not just for appearance because it tells the system how the different parts of the configuration are connected. If I accidentally use a Tab or put something at the wrong indentation level, Docker Compose may not understand the file and the deployment can fail. This made me realize that small formatting mistakes can sometimes cause bigger problems.

The environment variables were another important part of the activity. Variables such as `MYSQL_DATABASE`, `MYSQL_USER`, and `MYSQL_PASSWORD` provide the information needed by the database and Nextcloud containers. They make it easier to pass configuration values to the containers without changing the actual application code. Docker Compose supports environment variables directly through the Compose configuration. :contentReference[oaicite:3]{index=3}

I was also surprised by how quickly Nextcloud could be deployed. After creating the Compose file and running the command, I was able to open the Nextcloud installation page in the browser. It made the activity feel more like a real cloud deployment instead of just a simple classroom exercise.

Since Mission 1, my understanding of cloud computing has changed. Before, I mostly thought of cloud computing as online storage and services. Now I understand that there is infrastructure behind these services, including containers, databases, networking, and application servers. This mission showed me that cloud computing also involves designing and managing the systems that make applications work.
