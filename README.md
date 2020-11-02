# AOS-CX-AWX-API-LAB
Lab working on Aruba OX CX with AWX, via APi

Engineer: [Andy Partridge](mailto:andy.partridge@roctechnologies.com)


Play builds the configuration for the following

Validate configurations

Version control

0.1 = 29/10/2020 final draft

Process
=======




Installation
============

Requires ansible 2.9.9 or later
No dependencies on other modules
There is no github pull for this code

useful
yum install tree
yum install telnet



Usage
=====

1) Inventory needs updating with the site,
2) A variable file for each Overlay, each switch config within.
3) Configs are overwritten within these folders on each pass
4) The main playbooks is `main.yaml` : use it to generate the entire config.
For example
`ansible-playbook main.yaml`

This runs the dist.j2 template,

Inventory based on hostname, can be used to limit to single sites
`ansible-playbook main.yaml -l aglc`


Work in Progress
================


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
