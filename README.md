deploy_netbox
=========

Ansible role to install Netbox 

Requirements
------------
Pip, Docker and Git needs be installed. All of which can be done so using the role.Docker can be installed using following role:

respiro.install_docker


Role Variables
--------------
All the  variables are listed in default folder. Some of the variables used are listed below:

netbox_base_dir : Directory path to install netbox
netbox_admin_email : set admin email
netbox_admin_username: set admin username
netbox_admin_password: set admin password

Dependencies
------------
VM is needed to install. Tested with following OS:

Ubuntu 18.04 (Bionic)

Example Playbook
----------------

    - hosts: servers
      become: yes
      roles:
         - role: respiro.deploy_netbox

License
-------

MIT / BSD

