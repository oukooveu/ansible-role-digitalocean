Ansible role: DigitalOcean
=========

Setup DigitalOcean droplet and SSH keys.

DigitalOcean API token should be provided through  `DO_API_TOKEN` environment variable.

Requirements
------------

None.

Role Variables
--------------

```
do_image: 'centos-7-x64'
do_size: '1gb'
do_region: 'ams3'
do_ssh_keys: []
```

Dependencies
------------

None.

Example Playbook
----------------

```
- hosts: localhost
  connection: local
  gather_facts: false
  roles:
    - digitalocean
```

License
-------

Apache 2.0

Author Information
------------------

Daniil Kupchenko, kupchenko@gmail.com
