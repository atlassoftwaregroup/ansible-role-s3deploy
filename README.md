s3deploy
========

Deploys tar files via rsync and s3cmd

Requirements
------------
None

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

- jnakatsui.s3cmd

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: jnakatsui.s3deploy }

License
-------

MIT

Note
----
Assumes that tar command is run inside directory

Set app though --extra-vars or -e when calling playbook
Always creates /opt/apps/{{ app }}

deploy_key: "full path to object in aws bucket not including bucket name"
