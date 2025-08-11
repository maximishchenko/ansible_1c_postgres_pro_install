Role Name
=========

This role provide installation PostgreSQL for 1C from PostgresPro

Requirements
------------

This role does not have any requirements

Role Variables
--------------

* postgres_password: postgres user password for setup (*required)
* app_1c_password: 1C application user password for setup (*required)
* app_1c_user: 1C application user name (optional, default: app1c)
* postgresql_1c_version: version of PostgreSQL for installation (optional, default: 17)

Dependencies
------------

This role does not have any dependencies

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```
---
  - hosts: all
    roles:
        - { role: 1c_postgres_pro_installation }
```

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```
  - hosts: servers
    roles:
        - { role: username.rolename, postgres_password: "...", app_1c_password: "..." }
```

License
-------

GPLv3

Author Information
------------------

Maxim Ishchenko <m.g.ishchenko@gmail.com>
