# server_config
Installation of a Linux distribution on a virtual machine (Amazon lightSail) and prepare it to host your web applications, to include installing updates, securing it from a number of attack vectors and installing/configuring web and database servers.

## IP Address
13.127.106.247

## SSH Port
2200

## URL
http://ec2-13-127-106-247.ap-south-1.compute.amazonaws.com/

## Installations and configurations
- Updated all currently installed packages
- Changed the SSH port from 22 to 2200
- Configured the Uncomplicated Firewall (UFW) to only allow incoming connections for SSH (port 2200), HTTP (port 80), and NTP (port 123).
- created a new linux user `grader`, with the ability to do sudo. And Created an SSH key pair for `grader` using the ssh-keygen tool.
- Apache Server
- mod_wsgi
- PostgreSQL, created a new database user `catalog` having previlages for `catalog` database.
- git
- Python flask
- Python SQLAlchemy
- psycopg2
- Configured `catalog- Restaurant-menu` project to be accessable at port 80 of server
