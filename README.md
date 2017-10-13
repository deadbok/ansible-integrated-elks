Ansible roles to install a monolithic monitoring server running elastic stack
and librenms. *This role has only been tested on Debian*

# Monitoring server

Ansible script to deploy a logserver performing the following tasks:

 * Update packages.
 * Install openjdk-8-jre
 * Install Elasticsearch
 * Install Logstash
 * Install Kibana
 * Install ufw
 * Install open-vm-tools
 * Install the Midnight Commander
 * Instlal the nano editor

 * Close all ports except 22, 80 using ufw
