Ansible Role for AWS SSM installation
=========

This role install and configure AWS SSM agent on linux cento 7. 
Feel free to contribute by adding more linux distro, release and architecture. 

Requirements
------------

- CentOS 7 / Redhat 7


Role Variables
--------------

| Name|Default|Description |
| :--- | :---:| :--- |
|ssm_dnl_dir|/tmp|Download directory|
|ssm_pkg_name|amazon-ssm-agent.rpm|AWS SSM package name|
|ssm_pkg_url|https://s3.amazonaws.com/ec2-downloads-windows/SSMAgent/latest|Download URL|
|ssm_svc_state|started|SSM service state|


Dependencies
------------

None

Example Playbook
----------------


    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

