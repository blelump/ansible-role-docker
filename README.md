marklee77.docker
================

[![Build Status](https://travis-ci.org/marklee77/ansible-role-docker.svg?branch=master)](https://travis-ci.org/marklee77/ansible-role-docker)

Role to install Docker on various distributions, particularly Ubuntu, Debian,
Fedora and CentOS. Debian distributions use the docker.io repository, while
RedHat distributions use standard repositories.

This playbook is implemented using a common set of tasks customized by
os-specific variables. This means that if there are multiple systems with
different operating systems, docker will be installed in parallel rather than
sequentially (as would be the case if using include: ... when: ...).

Example Playbook
-------------------------

    - hosts: all
      roles:
        - marklee77.docker

License
-------

GPLv2

Author Information
------------------

http://stillwell.me
