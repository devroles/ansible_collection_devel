oasis_work
===========

Prepares a system to work on OASIS roles. Requires that the
`ansible` role from this collection also be run before this
one.

Requirements
------------

Ansible 2.8 or higher

Red Hat Enterprise Linux 7 or equivalent

Valid Red Hat Subscriptions

Role Variables
--------------

Currently the following variables are supported:

### General

* `oasis_work_prefix` - Default: `ansible_user_dir`. The path prefix where
you want repositories to be checked out and paths to be set

Dependencies
------------

None

Example Playbook
----------------

```yaml
- hosts: oasis_work-servers
  roles:
    - role: devroles.devel.ansible
    - role: devroles.devel.oasis_work
```

License
-------

GPLv3

Author Information
------------------

Greg Hellings
