Common Configuration for multiple OS
=========

This ansible role configure users, groups, firewall, packages, ... for new installations

Requirements
------------

For windows, you need configure winrm because ansible use it to connect on server.
For linux, ssh server must configured to connect on server.
You have the choice to use the account "root" or a dedicated account with sudo or not. There are no
prerequiste for this role.

Role Variables
--------------


defaults/main.yml: this file contains variables for groups and users.
vars/rocky.yml: this file contains variables for os Rocky Linux as packages, firewalld, ...

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: ansible-role-common
License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
