
```markdown
# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

For this laboratory, I worked with Docker Compose to create a private cloud storage environment using Nextcloud.

The setup used two containers. The first container was for MariaDB, which handled the database, while the second container was for Nextcloud, which provided the web interface.

I also learned how the two containers communicate with each other using the settings inside the Compose file.

## Objectives

The main objectives of this laboratory were:

- Learn the basic idea of Two-Tier Architecture.
- Create a Docker Compose configuration.
- Deploy MariaDB and Nextcloud together.
- Connect the Nextcloud application to the MariaDB database.
- Check the status of running containers.
- Access the Nextcloud setup page through port 8080.
- Properly stop and remove the containers after testing.

## Commands Executed

The following commands were used during the activity:

```bash
docker --version
