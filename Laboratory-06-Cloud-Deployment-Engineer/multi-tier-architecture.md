# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A two-tier architecture is a system divided into two main parts: the web/application tier and the database tier. The web/application tier handles user requests, while the database tier stores the application's data.

## Web/Application Tier

The web/application tier is responsible for serving the user interface and handling HTTP requests. In this activity, Nextcloud will be used as the web/application tier.

## Database Tier

The database tier is responsible for storing persistent data. This includes user accounts, settings, and other information needed by the application. In this activity, MariaDB will be used as the database tier.

## Why Separate Them?

Separating the web application and database into different containers makes the system easier to manage and maintain. Each container can focus on a specific role, and changes to one service can be made without directly affecting the other service.

Using separate containers also makes the architecture more organized and allows the services to communicate through the Docker Compose network.

