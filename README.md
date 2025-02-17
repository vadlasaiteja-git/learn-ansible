

## Getting started with Ansible
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

