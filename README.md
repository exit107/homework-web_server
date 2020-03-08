homework-web_server
=========

This role installs Apache and also copies in a replacement index.html.

Requirements
------------

None

Role Variables
--------------

None

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: homework-web_server }
