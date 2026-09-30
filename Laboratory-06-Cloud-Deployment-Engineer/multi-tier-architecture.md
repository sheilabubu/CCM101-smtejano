# Two-Tier Architecture

A **Two-Tier Architecture** is a system that separates an application into two main parts: the **Web/Application Tier** and the **Database Tier**. In this setup, the two parts work together but run separately, making the application easier to manage and maintain.

## The Web/Application Tier

The Web/Application Tier is responsible for serving the user interface and handling requests from users. In this laboratory, **Nextcloud** serves as the web application that users access through a web browser. It processes HTTP requests and provides the interface for uploading, managing, and accessing files.

## The Database Tier

The Database Tier is responsible for storing and managing persistent data needed by the application. In this laboratory, **MariaDB** is used as the database. It stores information such as user accounts, settings, and file metadata used by Nextcloud.

## Why Separate Them?

Separating the web application and database into two containers makes the system easier to manage, update, and troubleshoot. It also allows each container to focus on its specific role and makes it easier to scale or replace one part without affecting the other.

