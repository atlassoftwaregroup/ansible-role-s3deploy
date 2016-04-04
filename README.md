s3deploy
========

Deploys tar files via rsync and s3cmd

Requirements
------------
None

Role Variables
--------------

If deploy_access_key is undefined then IAM roles will be used.

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
The source code is licensed under GPL v3

Note
----
Assumes that tar command is run inside directory

Set app though --extra-vars or -e when calling playbook
Always creates /opt/apps/{{ app }}

deploy_key: "full path to object in aws bucket not including bucket name"
