# AOS-CX-AWX-API-LAB
Lab working on Aruba OX CX with AWX, via APi

Author: [Andy Partridge](mailto:andy.partridge@roctechnologies.com)


OVERVIEW
Plays are a lab to running automation on a Campus network - Aruba OS CX based.

All plays a work in Progress

Version control - draft work in progress

Play List
- main - Test connectivity and modules intergration
- ntp-heal - check the state of ntp and fix if not enabled
- pim-heal - Check pim is enabled and working, fix if not
- checkpoint - Enable checkpoint, make a change, and confirm access. If access, confirm checkpoint.






Installation Notes
==================

Requires ansible 2.9.9 or later
Requires - https://galaxy.ansible.com/arubanetworks/aoscx_role


useful
ansible-galaxy install arubanetworks.aoscx_role
yum install tree
yum install telnet



Ansible Installation
====================

sudo yum install upgrade
sudo yum install epel-release
sudo yum install ansible

AWX Installation
================


## Install AWX dependencies
yum install -y python3-pip
pip3 install ansible
pip3 install selinux #in case of selinux is enabled
pip3 install docker-compose #this is required even we installed docker-compose before.

# docker checker
docker container ls
