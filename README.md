# ansible-ldap-replicated
Ansible deployment of master-master replicated LDAP on Ubuntu 14.04

## Description

The is dual replication, writes to either server will be replicated to the other. 
Both sides are master and slave. 

## To create in vagrant:
Vagrant uses "hostmanager" plugin. Before running, install with: vagrant plugin install vagrant-hostmanager

`vagrant up`

ldap service available at:

`ldap1.internal.tld:389`

and

`ldap2.internal.tld:389`

username: admin@example.com pass: password
dc: example.com

edit `inventory/group_vars/all.yml` to change passwords

