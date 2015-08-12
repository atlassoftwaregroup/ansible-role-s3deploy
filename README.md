s3deploy
========

Deploys tar files via rsync and s3cmd

Requirements
------------
None

Role Variables
--------------

s3deploy-iam: If true does not look for aws access credentials. If false does look for aws access credentials

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
