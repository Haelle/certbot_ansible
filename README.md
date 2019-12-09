Role Name
=========

This Ansible role update Nginx configuration for a list of domains

Requirements
------------

Only works with Nginx

Role Variables
--------------

1. `domains_to_cert`: a list of domains to generate the certificates for
2. `certbot_admin_email`: e-mail of person in charge of these domains


Example Playbook
----------------

```yaml
- hosts: servers
  roles:
    - role: haelle.certbot_ansible
      certbot_admin_email: admin@example.com
      domains_to_cert:
        - an.example.com
        - another.example.com
```

License
-------

BSD
