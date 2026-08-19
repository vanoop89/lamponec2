# LAMP On EC2 Instances
This Ansible Repository helps to deploy the LAMP server on EC2 Instances. Using this you can automate instance deployment and deploy LAMP with WordPress installed on EC2 instances. 

# Architecture 
1. AWS Cloud
   - 2 EC2 Instances, one for WebServer and the other for Database 
   - 2 Security Groups
      - One to allow WebServer access on ports 80 and 443, and also allow SSH connection on port 22.
      - The other one is for the Database instance, it allows connections on port 3306 from the WebServer's SG and also allows SSH connections on 22.
2. LAMP
   - Apache/HTTPD Service
   - PHP
   - MariaDB
   - WordPress 
