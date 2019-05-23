systemd_resolved
================

An Ansible Role that disable systemd-resolved.

Role Variables
--------------

Available variables are listed below, along with default values (see
`defaults/main.yml`):

```yaml

search_domain: example.com
nameserver1: 1.1.1.1
nameserver2: []

```

Dependencies
------------

None.

Example Playbook
----------------

```yaml

- name: Disable systemd-resolved
  hosts: [all]
  become: yes

  roles:
    - role: gcoop-libre.systemd_resolved
      search_domain: example.com
      nameserver1: 1.1.1.1

```

License
-------

GNU General Public License, GPLv3

Author Information
------------------

This role was created in 2019 by
 [Osiris Alejandro Gomez](https://osiux.com/),
 worker cooperative of
 [gcoop Cooperativa de Software Libre](http://www.gcoop.coop/).
