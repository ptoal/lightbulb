Ansible Vagrant training provisioner
================================

This is an automated lab setup for Ansible training. It creates five nodes per user in the `users` list.

* One control node from which Ansible will be executed from and where Ansible Tower can be installed
* Three web nodes that coincide with the three nodes in lightbulb's original design
* And one node where `haproxy` is installed (via lightbulb lesson)

## Usage ##


### Vagrant Setup ###

To set up the lab for Ansible training, follow these steps.

1. Install Vagrant (>=v1.8.0) and VirtualBox.

2. Run:

   "vagrant up"

3. After provisioning is finished, run:

   "vagrant ssh control"
   >sudo -i su - ansible-user


### Vagrant Teardown ###


1. Run:

   "vagrant destroy -f"
