Role Name
========

sslkeys

Role Variables
--------------
```
# Enable this role, turn this off by default to minimize risk of exposing keys
manage_ssl: false
# Directory ssl keys will be copied to unless specified
ssl_key_dir: /etc/ssl/private/
# SSL key location, where the keys are located to deploy.
ssl_key_loc: ssl/

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
