# Prometheus Deployment with Ansible and Vagrant

This repository provides the necessary files and playbooks to deploy Prometheus, an open-source monitoring and alerting toolkit, using Ansible and Vagrant. The deployment is designed to be performed between two Vagrant virtual machines.

## Prerequisites

Before deploying Prometheus, ensure that you have the following:

- Vagrant installed on your machine.
- Ansible installed on the machine from where the deployment will be orchestrated.

## Getting Started

To deploy Prometheus using Ansible and Vagrant, follow these steps:

1. Clone this repository to your local machine.
2. Navigate to the repository directory.
3. Start the Vagrant virtual machines by executing the following command:

```shell
vagrant up
Update the inventory.txt file with the IP addresses or hostnames of the Vagrant virtual machines.
Modify the template.yml playbook according to your specific requirements.
Execute the ansible-playbook command, providing the appropriate inventory file:
ansible-playbook template.yml -i inventory.txt
Sit back and let Ansible handle the deployment process.
