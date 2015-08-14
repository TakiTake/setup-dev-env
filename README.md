Setup development environment with docker-toolbox
=================================================

Local => MacBook Air, Remote => Ubuntu14.04 on SakuraVPS

You only have to add working user to Remote Server. This Ansible script install docker with docker-machine and cluster docker hosts with docker-swarm.

Setup
-----

- Install (docker-toolbox)[https://www.docker.com/toolbox]
- Install (Ansible)[http://www.ansible.com/home]

```
# Change remote host name
$ vim hosts

# Change username and IP
$ vim group_vars/all.yml

$ ansible-playbook -i hosts --ask-pass --ask-sudo-pass site.yml
```
