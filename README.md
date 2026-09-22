# AWS LAMP Stack WordPress Project

## Project Overview

This project covers the deployment of a WordPress website on an Ubuntu-based Amazon EC2 instance.

The EC2 instance was configured with Apache and PHP to host the WordPress application. Amazon RDS was used as the MySQL database, keeping the application and database on separate services.

## Project Architecture

The deployment consists of the following components:

- Amazon EC2 – Application and web server
- Ubuntu – Operating system
- Apache – Web server
- PHP – Application runtime
- WordPress – Website application
- Amazon RDS – MySQL database
- MySQL Client – Database connectivity and testing

## Implementation

### 1. EC2 Instance Setup

An Ubuntu EC2 instance was prepared to host the WordPress application. The instance was accessed through the AWS EC2 Instance Connect environment.

![EC2 Web Server Setup](EC2-WebServer-Setup.png.png)

### 2. Ubuntu System Update

The Ubuntu system was updated before installing and configuring the required application packages.

![Ubuntu System Update](Ubuntu-System-Update-and-Restart-Check.png.png)

### 3. Apache Web Server

Apache was installed on the EC2 instance and configured as the web server for the WordPress application.

The Apache service was checked to verify that it was running correctly.

![Apache Service Status](Apache-Service-Status.png.png)

### 4. MySQL Client Installation

The MySQL client was installed on the EC2 instance to provide command-line access for testing the database connection.

![MySQL Client Installation](Install-MySQL-Client.png.png)

### 5. Database Connectivity

The MySQL client was used to connect to the database and verify connectivity from the EC2 instance.

![MySQL Client Connection](MySQL-Client-Connection.png.png)

### 6. WordPress Database Configuration

WordPress was configured to use the database hosted on Amazon RDS.

The WordPress database configuration was updated with the required database name, username, password, and RDS endpoint.

![WordPress Database Configuration](WordPress-Database-Configuration.png.png)

### 7. WordPress Configuration

The WordPress configuration file was reviewed and the required application and security settings were configured.

![WordPress Configuration](WordPress-Configuration-Security-Settings.png.png)

### 8. WordPress Installation

After completing the server and database configuration, the WordPress installation page was accessed through the web server.

![WordPress Installation](Wordpress-Signup-page.png.png)

### 9. WordPress Website

The WordPress installation was completed and the website was accessed successfully through the EC2-hosted web server.

![WordPress Home Page](Wordpress-Home-page.png.png)

## Project Result

The WordPress application was deployed successfully on an Ubuntu EC2 instance using Apache and PHP, with Amazon RDS providing the MySQL database.

The project also provided hands-on experience with configuring a web server, connecting an application to a remote database, and troubleshooting connectivity and application configuration issues.

## Key Learnings

- EC2 instance setup and management
- Ubuntu server administration
- Apache web server configuration
- PHP installation and configuration
- WordPress deployment
- Amazon RDS and MySQL connectivity
- WordPress database configuration
- Basic Linux troubleshooting
- Application and database connectivity testing
- Project documentation using GitHub
