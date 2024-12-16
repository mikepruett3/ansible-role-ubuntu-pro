Ansible Role: Ubuntu Pro Subscription
=========

Ansible role to configure Ubuntu Pro subscription settings on Linux Servers.

Requirements
------------

The role does not require anyting to run on Ubuntu servers.

Role Variables
--------------

Available variables are listed below, along with default values (see ```defaults/main.yml```):

``` yaml
username: "myuser"
password: "mypass"
activation_key: "xxxxxxxxxx"
spacewalk_server: "myserver.example.com"
```

```username``` The username for Red Hat Enterprise Subscription Manager account

```password```  The password for Red Hat Enterprise Subscription Manager account

```activation_key```  The activiation key to use with SpaceWalk Server

```org_id```  The Organization ID to use with SpaceWalk Server (Normally "1")

```spacewalk_server```  The hostname of the SpaceWalk Server

Role variables can be stored with the hosts.yaml file, or in the main variables file.

Dependencies
------------

None.

Example Playbook
----------------

``` yaml
    - hosts: servers
      roles:
         - role: mikepruett3.ubuntu-pro
```

License
-------

MIT

Author Information
------------------

Role created by [mikepruett3](https://github.com/mikepruett3) on [Github.com](https://github.com/mikepruett3/ansible-role-ubuntu-pro)
