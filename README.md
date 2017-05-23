Role Base
=========
[![N|Solid](https://www.softexia.com/wp-content/uploads/2015/11/Windows_Server_logo.png)](https://www.microsoft.com/es-es/WindowsForBusiness/)

This role configures basic setting in SO, like install Nutanix Guest Tools and join windows server to a AD domain.

Requirements
------------

A Windows 2008 R2 or higher.

Role Variables
--------------
- Defaults/main.yml
    - dns: 
        dns_name: domain name
    - repo:
        basePath: base path to the software windows repository
        NutanixGT: relative path to Nutanix Guest Tools exe.
   
    - debug: (true/false) sets debug on / off
    
- Defaults/users.yml (Encrypted!!!)
    - users: 
        dns_account_user: (must have enough priviledges to join a server to the domain)
           user: username
           password: password



Example Playbook
----------------



Author Information
------------------

Informática El Corte Inglés