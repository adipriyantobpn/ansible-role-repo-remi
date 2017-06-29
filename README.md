Ansible Role: REMI Repository
=========

An Ansible Role that to manage REMI Yum repository

Requirements
------------

This role needs no special requirements, except sudo access

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):


```yaml
---
repo_location:              indonesia   # available options: international, indonesia, vagrant
remi_enabled:               no
remi_safe_enabled:          yes
remi_php54_enabled:         no
remi_php55_enabled:         no
remi_php56_enabled:         no
remi_php70_enabled:         no
remi_php71_enabled:         yes
```

Dependencies
------------

None

Example Playbook
----------------

```yaml
---
- name: Prepare CentOS 7 server
  hosts: centos7
  roles:
    - role: adipriyantobpn.repo-remi
      repo_location:              international
      remi_enabled:               no
      remi_safe_enabled:          yes
      remi_php54_enabled:         no
      remi_php55_enabled:         no
      remi_php56_enabled:         no
      remi_php70_enabled:         no
      remi_php71_enabled:         yes
```

License
-------

BSD

Author Information
------------------

This role was created in 2017 by [Adi Priyanto](https://github.com/adipriyantobpn) as a learning purpose for community.