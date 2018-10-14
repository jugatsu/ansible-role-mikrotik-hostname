ansible-role-mikrotik-hostname
=========

An Ansible Role that configures hostname on MikroTik routers (https://mikrotik.com).

:point_up: You can use https://github.com/jugatsu/packer-mikrotik to build Vagrant box for testing this role.

Requirements
------------

This role only supports ansible 2.7.

Role Variables
--------------

Hostname of router:

`mikrotik_hostname: "MikroTik"`


Example Playbook
----------------
```yaml
- hosts: routers
  roles:
    - { role: ansible-role-mikrotik-hostname }
```

How to test role
----------------

Install pipenv (https://github.com/pypa/pipenv) and use this commands:

```bash
pipenv install
pipenv shell
vagrant up --provision
```

License
-------

BSD
