1c_postgres_pro_installation
=========

This role provide installation PostgreSQL for 1C from Postgres Professional

Role Variables
--------------

* `postgres_password`: postgres user's password for setup, if not set - will be generated
* `app_1c_password`: 1C application user's password for setup, if not set - will be generated
* `app_1c_user`: 1C application user name. Default: `app1c`
* `postgresql_1c_version`: version of PostgreSQL for installation. Default: `17`

Example Playbook
----------------

Including an example of how to use your role (for instance, without variables passed in as parameters):

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
        - { role: username.rolename, postgresql_1c_version: 17, postgres_password: "postgresuserpassword", app_1c_user: "onecuser", app_1c_password: "onecpassword" }
```

License
-------

GPLv3

Author Information
------------------

Maxim Ishchenko <m.g.ishchenko@yandex.ru>
