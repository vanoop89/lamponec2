EC2 Instance Deploy
=========

This role will create new EC2 Instances in the specified region.

Requirements
------------

This role used the Ansible collection amazon.aws so make sure this collection is installed on Ansible Controller before running this role. 
#ansible-galaxy collection list
#ansible-galaxy collection install amazon.aws


Role Variables
--------------

The role uses variable to set name of different resources that this role creates, so you need define them before running the role. All the user defined variables are defined in file defaults/main.yml, check and update it. 

Dependencies
------------

Nil

Example Playbook
----------------

Include this role in main playbook as below to create EC2 Instances.

    - hosts: localhost
      roles:
         - deploy-ec2

License
-------

Nil

Author Information
------------------

Name: Anoop V
Email: iamlinuxx@gmail.com
