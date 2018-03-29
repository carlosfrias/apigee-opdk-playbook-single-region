# Apigee OPDK Installation and Maintenance

This repository contains Ansible playbooks that use roles to install, configure and maintain Apigee Edge, Developer Portal and the 
Monitoring Dashboard. These playbooks orchestrate the usage of the roles to achieve the installation, upgrade and maintenance 
of the Edge platform. The roles perform functionally discrete activities. This is important because many installation, 
configuration and maintenance activities are multiple invocations of the same scripts or commands except for changes in
either the parameters used, the sequence of the invocations or both. Please see the links below for descriptions and 
instructions specific to your activity.  

## General Usage Instructions

Ansible playbooks are invoked at the command line. The assumption is that you know Ansible or are capable of learning Ansible 
quickly. 

### Ansible Playbooks
Ansible playbooks are always invoked using `ansible-playbook`. Please 
refer to [Ansible Documentation](http://docs.ansible.com/ansible/latest) for details on installing and running Ansible.

### Ansible Tags
These playbooks use [Ansible tags](http://docs.ansible.com/ansible/latest/cli/ansible-playbook.html#cmdoption-ansible-playbook-tags) 
extensively to execute functionally significant portions of the installation. These tags have been used consistently across all
the playbooks. In some cases, the tags perform slightly different tasks but achieve the semantic functionality ascribed by the name. 

| Tag Name | Description |
| --- | --- |
| cache | Updates the local Ansible cache with OPDK variables that are used for the generation of configuration files. |
| os | Prepares the operating system for the installation of OPDK as covered in the [Edge Installation Overview](https://docs.apigee.com/private-cloud/v4.18.01/installation-overview) and [Install the Edge Apigee Setup Utility](https://docs.apigee.com/private-cloud/v4.18.01/install-edge-apigee-setup-utility). This covers operating system packages and updates to system configuration files. |
| bootstrap | Install the Apigee bootstrap. This adapts to either [online](https://docs.apigee.com/private-cloud/v4.18.01/install-edge-apigee-setup-utility#installedgeapigeesetuputilityonanodewithanexternalinternetconnection) or [offline](https://docs.apigee.com/private-cloud/v4.18.01/install-edge-apigee-setup-utility#installedgeapigeesetuputilityonanodewithnoexternalinternetconnection) |
| common | Install [common](https://docs.apigee.com/private-cloud/v4.18.01/install-edge-apigee-setup-utility) Apigee components used on all nodes. This does not include operating system packages |
| config | Generate the [Edge Configuration File](https://docs.apigee.com/private-cloud/v4.18.01/edge-configuration-file-reference) |
| ds | Install the [ds](https://docs.apigee.com/private-cloud/v4.18.01/install-edge-components-node#specifyingthecomponentstoinstall) profile | 
| ms | Install the [ms](https://docs.apigee.com/private-cloud/v4.18.01/install-edge-components-node#specifyingthecomponentstoinstall) profile | 
| rmp | Install the [rmp](https://docs.apigee.com/private-cloud/v4.18.01/install-edge-components-node#specifyingthecomponentstoinstall) profile | 
| r | Install the [r](https://docs.apigee.com/private-cloud/v4.18.01/install-edge-components-node#specifyingthecomponentstoinstall) profile | 
| mp | Install the [mp](https://docs.apigee.com/private-cloud/v4.18.01/install-edge-components-node#specifyingthecomponentstoinstall) profile | 
| qpid | Install the [qs](https://docs.apigee.com/private-cloud/v4.18.01/install-edge-components-node#specifyingthecomponentstoinstall) profile | 
| pg | Install the [ps](https://docs.apigee.com/private-cloud/v4.18.01/install-edge-components-node#specifyingthecomponentstoinstall) profile |
| org | [Onboard an organization](https://docs.apigee.com/private-cloud/v4.18.01/onboard-organization) |
| validate | [Validate](https://docs.apigee.com/private-cloud/v4.18.01/test-install) the installation |
| logs | Download the configuration files and logs on a node that contains an Apigee component | 
 
## Installing, Updating and Maintaining Apigee Components and Support Servers 
| Playbook Description (README's Available) | Playbook Name | Playbook Role Requirements |
| --- | --- | --- |
| [Install AIO](README-AIO-execution.md) | [install-edge-aio.yml](install-edge-aio.yml) | [install-edge-aio-requirements.yml](install-edge-aio-requirements.yml) |
| [Install Edge](README-install-edge.md) | [install-edge.yml](install-edge.yml) | [install-edge-requirements.yml](install-edge-requirements.yml) |
| [Upgrade Edge](README-upgrade.md) | [upgrade-edge.yml](upgrade-edge.yml) | [upgrade-edge-requirements.yml](upgrade-edge-requirements.yml) |
| [Apigee Bash Scripts Debug Mode](README-apigee-opdk-debug-mode.md) | [apigee-opdk-debug-mode.yml](apigee-opdk-debug-mode.yml) | [apigee-opdk-debug-mode-requirements.yml](apigee-opdk-debug-mode-requirements.yml) | 


##  Installing, Updating and Maintaining Apigee Components and Support Servers 
| Playbook Description (README's under construction) | Playbook Name | Playbook Role Requirements |
| --- | --- | --- |
| [Install Developer Portal](install-devportal.yml) | [install-devportal.yml](install-devportal.yml) | [install-devportal-requirements.yml](install-devportal-requirements.yml) |
| [Install Baas](install-baas.yml) | [install-baas.yml](install-baas.yml) | [install-baas-requirements.yml](install-baas-requirements.yml) |
| [Install Monitoring Dashboard](install-monitoring.yml) | [install-monitoring.yml](install-monitoring.yml) | [install-monitoring-requirements.yml](install-monitoring-requirements.yml) |
| [Install Apigee Mirror](install-mirror.yml) | [install-mirror.ym](install-mirror.yml) | [install-mirror-requirements.yml](install-mirror-requirements.yml) |
| [Install Monetization](install-monetization.yml) | [install-monetization.yml](install-monetization.yml) | [install-monetization-requirements.yml](install-monetization-requirements.yml) |
| [Add a Data Center to a Planet](edge-expansion.yml) | [edge-expansion.yml](edge-expansion.yml) | [edge-expansion-requirements.yml](edge-expansion-requirements.yml) |
| [Clean Control Server](clean.yml) | [clean.yml](clean.yml) | NA | 
| [Hard Remove of Apigee from a Node](apigee-node-rollback.yml) | [apigee-node-rollback.yml](apigee-node-rollback.yml) | NA |
| [Download Apigee Logs](apigee-log-config-files.yml) | [apigee-log-config-files.yml](apigee-log-config-files.yml) | NA |


<!-- BEGIN Google Required Disclaimer -->

# Not Google Product Clause

This is not an officially supported Google product.
<!-- END Google Required Disclaimer -->
