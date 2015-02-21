================
Ansible Workshop
================

.. class:: center

| Hands on Ansible deploying GitLab
| Location - Webonise Lab, Pune
| Date - 2015-02-21

.. footer:: Location - Webonise Lab, Pune

About Me
========

:Name: Rishabh Das
:Contact: rishabh5290@gmail.com
:Workplace: Red Hat, Pune

Agenda
======

- What is Ansible
- Installation
- Ansible modules
- Ansible variables
- Ansible playbook
- Demo

What is Ansible
===============

.. image:: Images/Ansible.png
    :height: 400px
    :width: 500px
    :scale: 50%
    :align: center

- IT automation tool
- Deploy, Manage and Configure applications

Installation
============

- RPM family - yum install ansible
- Debian / Ubuntu - apt-get install ansible
- pip install ansible

Ansible Modules
===============

- Control system resources
- Supports arguments
- Written in Python

Ansible Variables
=================

- Inventory variables
- Playbook variables
- Discovered variables or Facts

Ansible Playbook
================

- YAML file
- Set of instructions
- Has host details
- Variables to read from

Sample Playbook
===============

.. code:: yaml

   ---
   - name: install and start httpd service
     hosts: webservers
     user: cloud-user
     sudo: yes
     tasks:
        - name: Install / Check apache is intalled
          yum: name=httpd state=present
        - name: Start / Check apache service
          service: name=httpd state=started

Demo
====

.. class:: center

| 
| 
| 
| **Deploy GitLab**

Documentation
=============

- http://docs.ansible.com/
- http://docs.ansible.com/list_of_all_modules.html

Slides / Code
=============

- https://github.com/rishabhdas/GitLab-Ansible.git

Thank You
=========

| 
| 

.. image:: Images/ThankYou.png
    :align: center
