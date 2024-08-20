# Ubuntu 2204 Setup
Configures a new install of Ubuntu 22.04 and 24.04 using Ansible.

## Prerequisites
To utilise this script, you will need the following:
 - A fresh installation of either Ubuntu 22.04 or 24.04.
 - A DNS record which resolves to the installation.
 - An installation of Ansible on the machine you intend on executing this script.
 - An SSH key which utilises ed25519.

## Variables
The following variables need to be set within the playbook.yml file:
 - username

In addition to this, you can also add packages by adding to the `packages` variable.

## Inventory
In order for this script to work correctly, you will need to specify the hostname in the inventory file as this will be used to configure the server. 

## Running the setup
To run the script, run the following command:
`ansible-playbook playbook.yml -i inventory.yml -u root`
