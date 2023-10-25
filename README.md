Red Hat Ansible Training
---------------------------

Introduction 
--------------

Red Hat Ansible Training tries to give a general overview about Red Hat Ansible Automation Platform and Red Hat Ansible Automation Controller solutions, covering the most important concepts and elements inside these automation tools.

To support this objective, a set of practical laboratories have been included in this training in order to explore each point deeply and assist the student learning process to internalizing best practices and key concepts.

Folder Structure 
-----------------

A folder structure is provided in this repository in order to split laboratory content and improve the clarity of the training. The following folders have been included with a specific objective:

-   iac_tower -> Includes Red Hat Ansible Tower configuration as a code. 
-   examples -> Includes son Ansible playbooks and roles which could be useful in a future steps.
-   training -> Lessons structure which includes Red Hat Ansible Engine's specific exercises with solutions.
-   training_microsoft -> Lessons structure which includes specific Red Hat Ansible Tower's exercises focus on Azure environment and Microsoft Servers administration.

Laboratory Environment
------------------------

This lab is intended to be run in a local Vagrant machine. There may be
assumptions that you are running this on Ubuntu 22.04LTS so be mindful of the
some steps that include package names and some modules or commands. Largely
this should translate to other distributions as well.

These instructions will not guide yout through the installation of Vagrant and
any supported providers. This assumes you already have this set up.

First you need to start your Vagrant machine and connect to it:

- Start Vagrant machine
```
$ cd ~/vagrant/ubuntu && vagrant up
```

- Set up a Vagrant VM using Ubuntu 22.04LTS
```
$ mkdir -p ~/vagrant/ubuntu && cd ~/vagrant/ubuntu
```

- Initialize the Vagrant VM, if you have not done so already
```
$ vagrant init generic/ubuntu2204
```

- Start your Vagrant VM
```
$ vagrant up
```

- Connect to your Vagrant VM
```
$ vagrant ssh
```

- Clone this repository, if you haven't already
```
$ mkdir -p ~/git && cd ~/git && git clone https://github.com/barstown/ansible-training
```

Red Hat Ansible Engine Lessons
---------

Training folder includes The following list includes a lessons summary:

-   [**Lesson 1**](./training/lesson01/README.md) - Install Ansible
-   [**Lesson 2**](./training/lesson02/README.md) - Configure Ansible
-   [**Lesson 3**](./training/lesson03/README.md) - Ansible AdHoc Commands
-   [**Lesson 4**](./training/lesson04/README.md) - Ansible Inventory
-   [**Lesson 5**](./training/lesson05/README.md) - Ansible Playbooks
-   [**Lesson 6**](./training/lesson06/README.md) - Ansible Variable
-   [**Lesson 7**](./training/lesson07/README.md) - Ansible Facts
-   [**Lesson 8**](./training/lesson08/README.md) - Ansible Vault
-   [**Lesson 9**](./training/lesson09/README.md) - Ansible Conditionals, loops and delegation
-   [**Lesson 10**](./training/lesson10/README.md) - Ansible Handlers
-   [**Lesson 11**](./training/lesson11/README.md) - Ansible Templates
-   [**Lesson 12**](./training/lesson12/README.md) - Ansible Roles
-   [**Lesson 13**](./training/lesson13/README.md) - Ansible Filters
-   [**Lesson 14**](./training/lesson14/README.md) - Ansible Modules
-   [**Lesson 15**](./training/lesson15/README.md) - Ansible Lookups, Callbacks & Tags

Red Hat Ansible Tower Lessons
---------

Training folder includes The following list includes a lessons summary:

-   [**Lesson 1**](./training_tower/lesson01/README.md) - Install Ansible Tower
-   [**Lesson 2**](./training_tower/lesson02/README.md) - Credentials
-   [**Lesson 3**](./training_tower/lesson03/README.md) - Projects
-   [**Lesson 4**](./training_tower/lesson04/README.md) - Inventories
-   [**Lesson 5**](./training_tower/lesson05/README.md) - Job Templates
-   [**Lesson 6**](./training_tower/lesson06/README.md) - Workflow Templates
-   [**Lesson 7**](./training_tower/lesson07/README.md) - Ansible Tower Role Based Access Control
-   [**Lesson 8**](./training_tower/lesson08/README.md) - Emulate a Real Ansible Tower Project (Bonus)

Red Hat Automation Platform & Microsoft Training
---------

Please, visit [**Red Hat Automation Platform & Microsoft Training**](./training_microsoft/README.md) to access this training.


License
-------

BSD

Author Information
------------------

 Asier Cidon - Cloud Consultant

 asier.cidon@redhat.com
   
