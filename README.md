

# Getting started with Ansible
Ansible automates the management of remote systems and controls their desired state.

Most Ansible environments have three main components:

- Control node
A system on which Ansible is installed. You run Ansible commands such as ansible or ansible-inventory on a control node.

- Inventory
A list of managed nodes that are logically organized. You create an inventory on the control node to describe host deployments to Ansible.

- Managed node
A remote system, or host, that Ansible controls.


## Ansible playbooks
Ansible Playbooks offer a repeatable, reusable, simple configuration management and multi-machine deployment system, one that is well suited to deploying complex applications. If you need to execute a task with Ansible more than once, write a playbook and put it under source control. Then you can use the playbook to push out new configuration or confirm the configuration of remote systems.

Playbooks can:

- declare configurations

- orchestrate steps of any manual ordered process, on multiple sets of machines, in a defined order

- launch tasks synchronously or asynchronously

## Playbook syntax
Playbooks are expressed in YAML format with a minimum of syntax. If you are not familiar with YAML, look at our overview of YAML Syntax and consider installing an add-on for your text editor (see Other Tools and Programs) to help you write clean YAML syntax in your playbooks.

A playbook is composed of one or more ‘plays’ in an ordered list. The terms ‘playbook’ and ‘play’ are sports analogies. Each play executes part of the overall goal of the playbook, running one or more tasks. Each task calls an Ansible module.

## Playbook execution
A playbook runs in order from top to bottom. Within each play, tasks also run in order from top to bottom. Playbooks with multiple ‘plays’ can orchestrate multi-machine deployments, running one play on your webservers, then another play on your database servers, then a third play on your network infrastructure, and so on. At a minimum, each play defines two things:

- the managed nodes to target, using a pattern

- at least one task to execute