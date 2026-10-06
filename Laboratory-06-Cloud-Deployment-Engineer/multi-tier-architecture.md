
## What is a Two-Tier Architecture?

A Two-Tier Architecture divides an application into two main parts. One part handles the application and user interface, while the other part is responsible for storing and managing the application's data.

For this activity, Nextcloud is the application tier and MariaDB is the database tier.

## The Web/Application Tier

The web or application tier is where the main application runs. It receives requests from the user and provides the interface that the user sees in the browser.

In this project, the Nextcloud container acts as the web/application tier. It handles the web interface and allows users to access the private cloud storage through a browser.

## The Database Tier

The database tier is responsible for keeping the information used by the application. It stores data such as user accounts, database records, and other information needed by Nextcloud.

In this project, MariaDB is used as the database. It runs in a separate container from the Nextcloud application.

## Why Separate Them?

Keeping the application and database in separate containers makes the system easier to organize and maintain. If one part needs to be updated or changed, it can be managed without putting everything inside one container.

It also makes the setup easier to expand because the application and database can be managed independently.
