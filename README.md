# AOS-CX-AWX-API-LAB
Lab working on Aruba OX CX with AWX, via APi

Author: [Andy Partridge](mailto:andy.partridge@roctechnologies.com)


OVERVIEW
Plays are a lab to running automation on a Campus network - Aruba OS CX based.

All plays a work in Progress

Version control - draft work in progress

Play List
Main - Test conenctivity and modules intergration
Full-Validate - Take a copy of the config and MD5 has to confim no changes
ntp-heal - check the state of ntp and fix if not enabled
Checkpoint - Enable checkpoint, make a change, and confirm access. If access, confirm checkpoint.





Installation Notes
==================

Requires ansible 2.9.9 or later
Dependencies on on the arube modules
Uses both API and SSH

useful
yum install tree
yum install telnet



Ansible Installation
====================

sudo yum install upgrade
sudo yum install epel-release
sudo yum install ansible

AWX Installation

https://medium.com/swlh/ansible-awx-installation-5861b115455a

## Install AWX dependencies
yum install -y python3-pip
pip3 install ansible
pip3 install selinux #in case of selinux is enabled
pip3 install docker-compose #this is required even we installed docker-compose before.

# docker checker
docker container ls
