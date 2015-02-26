moodle
=========

Install moodle

Role Variables
--------------

    db_host: "127.0.0.1"
    db_pwd_root: "dificil"
    db_name: 'moodle'
    db_username: 'moodleAdmin'
    db_password: 'unaContrasenia'

    moodle_domain: "moodle.docker"
    moodle_path: "/opt/moodle"
    moodle_src: "{{ moodle_path }}/src"
    moodle_docs: "{{ moodle_path }}/moodleDocs"
    moodle_version: "MOODLE_28_STABLE"
    moodle_user: "moodle"

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
  - { role: krahser.moodle, moodle_version: "MOODLE_28_STABLE" }


License
-------

GPL-3

Author Information
------------------

Comments are welcome
