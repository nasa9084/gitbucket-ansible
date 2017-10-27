GitBucket-Ansible
=================

Ansible playbook to construct GitBucket Server on CentOS 7.

## Requirements

| App/Lib | Version  |
|:-------:|:--------:|
| Ansible | >= 2.2.0 |

## HOWTO

1. replace default to IP address or hostname (can be resolved via SSH) in `hosts`
2. replace passwords for MySQL root and GitBucket user in `roles/gitbucket/vars/main.yml`
3. run `$ ansible-playbook -i hosts site.yml`
4. if there's no errors displayed, now you can access to GitBucket with your server. the port is `:80`.
