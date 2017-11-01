osm_percona
=========

This is an ansible role of percona for Debian and RedHat Family.

Requirements
------------

There are no any pre-requisites or any requirment all you need is RedHat and Debian Machine.

Role Variables
--------------

The role variables are in [vars](https://github.com/opstree-ansible/osm_percona/blob/Release-1.1/vars/main.yml)

Dependencies
------------

The only dependency is MySQL-python

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: "{{ hosts }}"
      roles:
         - percona

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
