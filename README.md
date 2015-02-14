# Ansible Playbook

## Command

Show the list of defined tasks.
```
$ ansible-playbook -i hosts simple-playbook.yml --list-tasks

playbook: simple-playbook.yml

  play #1 (web):
    be sure httpd is installed
    be sure php is installed
    be sure httpd is installed
    be sure httpd is running and enabled

  play #2 (db):
    be sure Redis is installed.
    be sure mysqld is installed.
    be sure mysql is installed.
```

Dry-run execution.
```
$ ansible-playbook -i <inventory file> simple-playbook.yml --check
```

Execute playbook.
```
$ ansible-playbook -i <inventory file> simple-playbook.yml
```

