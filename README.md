# Udacity-Linux-Server
Details for viewing my Project 5 of Udacity's Fullstack Web Developer Nanodegree

## Connection Instructions


## Server Details
- IP Address:   52.37.195.167
- SSH Port:     2200
- URL:          http://ec2-52-37-195-167.us-west-2.compute.amazonaws.com

## Installed Software
- apache2
- python
- postgresql
- psycopg2
- python-sqlalchemy
- python-pip
- werkzeug==0.8.3
- flask==0.9
- Flask-Login==0.1.3
- oauth2client
- requests
- httplib2
- git

## Configuration Changes
- Created sudo user grader.
- Configured key based login.
- Disabled password login.
- Disabled remote login for root.
- Updated all currently installed packages.
- Changed the SSH port from 22 to 2200.
- Configured the Uncomplicated Firewall (UFW) to only allow incoming connections for SSH, HTTP, and NTP.
- Configured the local timezone to UTC.
- Created Linux user 'catalog' and postgresql user 'catalog' with same password.
- Created postgresql database 'catalog'.
- Configured Apache to run catalog app as a Python mod_wsgi application.
- Converted app from sqlite to postgresql.
- Converted app to use absolute file paths.
- Moved app.SECRET_KEY from main method into the body of the app.

## References
- Udacity Course, "Configuring Linux Web Servers."
- https://www.digitalocean.com/community/tutorials/how-to-configure-the-apache-web-server-on-an-ubuntu-or-debian-vps
- https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps
- https://discussions.udacity.com/t/running-apache-problem/35719/6
- https://discussions.udacity.com/t/operationalerror-unable-to-open-dat-abase-file-none-none/36401/4
- https://developers.facebook.com - Added server IP to whitelist and URL to Valid OAuth redirect URIs.
- https://console.cloud.google.com - Added JavaScript origins and OAuth redirect URIs.
