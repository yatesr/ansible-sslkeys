Role Name
========

sslkey-deploy

Role Variables
--------------
```
# Enable this role, turn this off by default to minimize risk of exposing keys
manage_ssl: false
# Directory ssl keys will be copied to unless specified
ssl_key_dir: /etc/ssl/private/

```

Example Playbook
-------------------------
### playbook.yml

```

---
- hosts: all
  roles:
  - sslkey-deploy

  vars:
    manage_ssl: true

```

License
-------

Apache 2.0

Author Information
------------------

Ryan Yates
