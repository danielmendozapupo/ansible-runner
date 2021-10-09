Execute the following command line instruction
$ ansible-runner run demo --playbook test.yml
```
[DEPRECATION WARNING]: Ansible will require Python 3.8 or newer on the 
controller starting with Ansible 2.12. Current version: 3.6.8 (default, Nov 16 
2020, 16:55:22) [GCC 4.8.5 20150623 (Red Hat 4.8.5-44)]. This feature will be 
removed from ansible-core in version 2.12. Deprecation warnings can be disabled
 by setting deprecation_warnings=False in ansible.cfg.

PLAY [all] *********************************************************************

TASK [Gathering Facts] *********************************************************
ok: [localhost]

TASK [include_role : testrole] *************************************************

TASK [testrole : just print a message to stdout] *******************************
ok: [localhost] => {
    "msg": "hello from the ansible-runner testrole!"
}

TASK [debug] *******************************************************************
ok: [localhost] => {
    "msg": "Test!"
}

PLAY RECAP *********************************************************************
localhost                  : ok=3    changed=0    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0
```
To use the python Script:

