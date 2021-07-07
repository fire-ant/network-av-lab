Role Name
=========

A role to apply some basic configuration to Cisco SG300 (And eventually other types of switch) to ensure that they are capable of supporting Dante Audio Network devices.

Requirements
------------

You need to use this against a valid Cisco SG300 switch. The role was developed using: 

molecule 3.3.4 using python 3.9 
    ansible:2.11.2
    delegated:3.3.4 from molecule

You will also need to enable ssh and configure a user with the publi half of an ssh key to provision access for ansible to use.

Role Variables
--------------

```
system_mode: switch|router
vlans: [] # the vlan configuration we want to pass the switch (tags etc) 
interfaces: [] # the interfaces we want to pass to the switch 
igmp: [] # the vlan specific IGMP we want to pass to the switch
```

for a full example see the molecule/default/molecule.yml or the defaults/main.yml 

Dependencies
------------

NA.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: fire-ant.dante, system_mode: switch }
License
-------

BSD

Author Information
------------------

reach out to me here on GH or through a PR to make this better.
