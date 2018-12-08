Ansible Role for AWS SSM installation
=========

[![Build Status](https://travis-ci.org/bitintheskud/ansible-role-ssm-agent.svg?branch=master)](https://travis-ci.org/bitintheskud/ansible-role-ssm-agent)

A very simple role to install and configure AWS SSM agent on linux (Centos 7 only  for now). 

Description
------------

This role install and configure AWS SSM agent on linux Centos 7. 

Contribution
------------

Please contribute by adding more linux distro, release and architecture ansible code.

Also, the travis build use [ansible-lint](https://github.com/ansible/ansible-lint) to enforce best practice. 


Requirements
------------

- Ansible 2.5 or higher


Role Variables
--------------

| Name|Default|Description |
| :--- | :--- | :--- |
|ssm_dnl_dir|/tmp|Download directory|
|ssm_pkg_name|amazon-ssm-agent.rpm|AWS SSM package name|
|ssm_pkg_url|https://s3.amazonaws.com/ec2-downloads-windows/SSMAgent/latest|Download URL|
|ssm_svc_state|started|SSM service state|


Dependencies
------------

- None


Example Playbook
----------------

```

--- 
   - hosts: localhost
     become: true
     roles:
       - ansible-role-ssm-agent
```

License
-------

BSD

Author Information
------------------

@bitintheskud 

