moodle
=========

Install moodle

Requirements
------------



Role Variables
--------------


Dependencies
------------

Roles dependecies:
- debops.pki
- debops.mysql
- debops.php5
- debops.nginx

Variables to setup:

- mysql
- php5
- nginx

Example Playbook
----------------

- hosts: Docker-devel
  roles:
  - { role: moodle, moodle_version: "MOODLE_28_STABLE" }


License
-------

GPL-3

Author Information
------------------

Comments are welcome
