# AWS LAMP Stack WordPress Project

## Project Overview

This project demonstrates the deployment of a WordPress website on an Ubuntu-based Amazon EC2 instance using a LAMP stack architecture.

The application server was configured on Amazon EC2 with Apache as the web server, PHP as the application runtime, and WordPress as the web application. Amazon RDS was used as the MySQL database service, keeping the application and database components separated.

The project covers the basic setup, configuration, database connectivity, WordPress configuration, and verification of the deployed website.

---

## Project Architecture

The deployment consists of the following components:

- Amazon EC2 – Application and web server
- Ubuntu Linux – Operating system
- Apache – Web server
- PHP – Application runtime
- WordPress – Web application
- Amazon RDS – MySQL database
- MySQL Client – Used to test database connectivity

### Architecture Flow

```text
                 Internet
                    |
                    v
             Amazon EC2
            Ubuntu Server
                    |
                    v
                Apache
                    |
                    v
              PHP / WordPress
                    |
                    v
             Amazon RDS MySQL
Implementation Steps
1. EC2 Web Server Setup

An Ubuntu-based Amazon EC2 instance was used as the application server.

The instance provides the compute environment required to host the Apache web server, PHP runtime, and WordPress application.

2. Ubuntu System Update

The Ubuntu server packages were updated before installing and configuring the application components.

Keeping the operating system packages updated helps provide a stable environment for the application deployment.

3. Apache Web Server

Apache was configured as the web server for the WordPress application.

The Apache service was checked using systemctl to confirm that the service was active and running.

4. MySQL Client Installation

The MySQL client was installed on the EC2 instance.

The client is used to connect from the application server to the MySQL database hosted on Amazon RDS.

5. MySQL Database Connectivity

After installing the MySQL client, a database connection was established to the MySQL server.

This step verified that the EC2 instance could communicate with the database service.

6. WordPress Database Configuration

WordPress was configured to use the MySQL database.

The database configuration includes the database name, database username, password, and database host.

The database host points to the Amazon RDS endpoint rather than a local MySQL database.

7. WordPress Configuration and Security Settings

The WordPress configuration file was reviewed and configured with the required application settings.

Security-related configuration, including WordPress authentication keys and salts, was also handled as part of the configuration process.

8. WordPress Setup

After configuring the application and database connection, the WordPress setup page was accessed through the web server.

This confirmed that the WordPress application was being served successfully from the EC2 instance.

![WordPress Setup](Wordpress Signup page.png.png)

9. WordPress Home Page

The final step was to verify the deployed WordPress website through the browser.

The WordPress home page confirmed that the web server, PHP application, WordPress files, and database configuration were working together.

![WordPress Home Page](Wordpress Home page.png.png)

Project Purpose

The purpose of this project was to gain practical experience in deploying a web application using AWS infrastructure.

The project demonstrates how an EC2 instance can be used as an application server while Amazon RDS provides a separate managed database service.

This approach separates the application and database layers and provides a foundation for further improvements such as load balancing, high availability, monitoring, and scaling.

Key Technologies
Technology	Purpose
Amazon EC2	Hosts the application
Ubuntu	Server operating system
Apache	Web server
PHP	WordPress application runtime
WordPress	Web application
Amazon RDS	Managed MySQL database
MySQL Client	Database connectivity and testing
What I Learned

Through this project, I gained practical experience with:

Launching and accessing an Ubuntu EC2 instance
Performing basic Linux server administration
Installing and managing Apache
Installing and using the MySQL client
Connecting an EC2 instance to an RDS MySQL database
Configuring WordPress to use an external database
Understanding the relationship between web, application, and database layers
Verifying services and troubleshooting deployment issues
Working with AWS resources through the AWS Management Console
Future Improvements

The current deployment can be extended into a more highly available architecture.

Possible improvements include:

Adding a second EC2 instance
Creating an Application Load Balancer
Configuring an EC2 Target Group
Using Auto Scaling
Improving database availability with appropriate RDS configuration
Adding Amazon CloudWatch monitoring
Configuring Route 53 for DNS management
Using HTTPS with AWS Certificate Manager
Conclusion

This project provides a practical example of deploying WordPress using an AWS-based LAMP architecture.

The application is hosted on an Ubuntu EC2 instance, while Amazon RDS provides the MySQL database layer. The implementation demonstrates the basic workflow from server preparation and web server configuration through database connectivity and WordPress deployment.


### Important: one filename needs attention

From your GitHub screenshot, these are the exact filenames:

- `EC2-WebServer-Setup.png.png`
- `Ubuntu-System-Update-and-Restart-Check.png.png`
- `Install-MySQL-Client.png.png`
- `MySQL-Client-Connection.png.png`
- `WordPress-Configuration-Security-Settings.png.png`
- `WordPress-Database-Configuration.png.png`
- `Apache-Service-Status.png.png`
- `Wordpress Signup page.png.png`
- `Wordpress Home page.png.png`

For the two filenames containing spaces, GitHub may handle them, but I recommend **renaming them to cleaner names**:

```text
WordPress-Setup-Page.png
WordPress-Home-Page.png
