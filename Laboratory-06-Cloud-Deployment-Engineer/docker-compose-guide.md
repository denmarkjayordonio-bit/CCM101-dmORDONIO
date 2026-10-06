# Docker Compose Guide

## What is Docker Compose?

Docker Compose is a tool that allows multiple containers to be configured and managed using one YAML file. Instead of creating every container separately, the required services can be written in one configuration file.

For this activity, the Compose file was used to create a Nextcloud application container and a MariaDB database container.

## The `services:` Block

The `services:` section contains the different parts of the application.

In our project, there are two services:

```yaml
services:
  database:
