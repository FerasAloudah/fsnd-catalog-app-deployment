## Project Description
You will take a baseline installation of a Linux distribution on a virtual machine and prepare it to host your web applications, to include installing updates, securing it from a number of attack vectors and installing/configuring web and database servers.

The server was deployed using [Amazon Lightsail](https://lightsail.aws.amazon.com), and [Apache2](https://httpd.apache.org/)

## Server Information
Server IP: 3.121.208.40

SSH Port: 2200

Web Application URL: http://3.121.208.40/

## Server Requirments
1. libapache2-mod-wsgi-py3.
2. Git.
3. PostgresSQL.
4. Everything inside requirments.txt from the original project.

##  Changes Made
 1. Updated all the installed packages.
 2. Configured the UFW to only allow incoming connections for SSH (port 2200), HTTP (port 80), and NTP (port 123).
 3. Disabled access to root.
 4. Created a new user named `grader` for the purpose of letting Udacity grade my project.
 5. Added `grader` to the sudo group, and generated a new ssh private key using `ssh-keygen`.
 6. Configured the local timezone to UTC.
 7. Installed PostgresSQL, added a new database and user for the sits.
 8. Created a `catalog.wsgi` file to connect my project with Apache2.
 9. Configured `catalog.conf` to edit everything needed to connect my project with Apache2.
 

## Outside Resources
1. [Deploy a Flask Application](https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps)
2. [Stueken's Repoistory](https://github.com/stueken/FSND-P5_Linux-Server-Configuration)
3. [PostgresSQL's setup](https://tecadmin.net/install-postgresql-server-on-ubuntu/)
