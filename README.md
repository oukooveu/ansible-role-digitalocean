Ansible role: DigitalOcean
=========

Setup DigitalOcean droplet and SSH keys.

DigitalOcean API token should be provided through `do_api_token` or `DO_API_TOKEN` environment variable.

Requirements
------------

None.

Role Variables
--------------

```
do_region: 'lon1'
do_ssh_keys: []
do_api_token: ''

droplet_image: 'centos-7-x64'
droplet_size: '1gb'
droplet_name: ''
droplet_inventory_groups:
  - digitalocean
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

Tasks
-----
- [ ] Setup firewall rules and attach it to droplet
- [ ] Setup basic monitoring for server/processes metrics
- [ ] Backup settings and implementation

License
-------

Apache 2.0

Author Information
------------------

Daniil Kupchenko, kupchenko@gmail.com
