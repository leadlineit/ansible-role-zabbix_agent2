# Ansible Role for Zabbix-Agent2 5.4

![Build Status](https://github.com/leadlineit/ansible-role-zabbix_agent2/actions/workflows/ansible-galaxy-ci.yml/badge.svg)
[![Galaxy Role](https://img.shields.io/badge/Ansible--Galaxy-leadlineit.zabbix_agent2-blue.svg?logo=ansible&logoColor=white)](https://galaxy.ansible.com/leadlineit/zabbix_agent2/)

This role helps to for install and configure Zabbix-Agent2 5.4 on a Debian (stretch/buster/bullseye).

Requirements
------------

This role requires Ansible 2.11 or higher.

Role Variables
--------------

```yaml
---
zabbix_agent_server: 127.0.0.1
zabbix_agent_listen_port: 10050
zabbix_agent_listen_ip: 0.0.0.0
zabbix_agent_psk: 6c4ccf50bacdb3486f141ba1112e4a46  # openssl rand -hex 16/(32)
```

All variables are optional, if you omit them the values above will be used (default).

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
- hosts: servers
  roles:
    - { role: leadlineit.zabbix_agent2, tags: zabbix_agent2 }
```

License
-------

MIT

Author Information
------------------

This role was created by Stas Stavnichuk.
