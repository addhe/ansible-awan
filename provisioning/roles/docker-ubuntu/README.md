Role Name
=========

Role to install docker-ce and docker-compose

Requirements
------------

No requirements

Role Variables
--------------

Default variables:
```
docker_compose_ver: declare default docker-compose version, default is 1.22.0
docker_ver: declare default docker-ce version, default is 18.09.6
docker_ver_pinning: declare docker-ce version pinning configuration template file, default is 'etc/apt/preferences.d/docker-ce.j2'
```

Dependencies
------------

No dependencies

Example Playbook
----------------

Example playbook
```
- hosts: "{{ target_hosts | default('all') }}
  vars_files:
    - inventory/group_vars/docker
  roles:
    - docker-image
```

License
-------

BSD

Author Information
------------------

Bukalapak System Engineer
