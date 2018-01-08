# Apigee OPDK Installation of a Single Data Center

This repository contains Ansible playbooks that use roles to install Apigee Edge, Developer Portal, Baas and the 
Monitoring Dashboard. These playbooks orchestrate the usage of the roles to achieve the following:
 
## Installing, Updating and Maintaining Apigee Components and Support Servers 
| Playbook Description | Playbook Name | Playbook Role Requirements |
| --- | --- | --- |
| [Install AIO](install-edge-aio.yml) | [install-edge-aio.yml](install-edge-aio.yml) | [install-edge-aio-requirements.yml](install-edge-aio-requirements.yml) |
| [Install Edge](install-edge.yml) | [install-edge.yml](install-edge.yml) | [install-edge-requirements.yml](install-edge-requirements.yml) |
| [Install Developer Portal](install-devportal.yml) | [install-devportal.yml](install-devportal.yml) | [install-devportal-requirements.yml](install-devportal-requirements.yml) |
| [Install Baas](install-baas.yml) | [install-baas.yml](install-baas.yml) | [install-baas-requirements.yml](install-baas-requirements.yml) |
| [Install Monitoring Dashboard](install-monitoring.yml) | [install-monitoring.yml](install-monitoring.yml) | [install-monitoring-requirements.yml](install-monitoring-requirements.yml) |
| [Install Apigee Mirror](install-mirror.yml) | [install-mirror.ym](install-mirror.yml) | [install-mirror-requirements.yml](install-mirror-requirements.yml) |
| [Install Monetization](install-monetization.yml) | [install-monetization.yml](install-monetization.yml) | [install-monetization-requirements.yml](install-monetization-requirements.yml) |
| [Add a Data Center to a Planet](edge-expansion.yml) | [edge-expansion.yml](edge-expansion.yml) | [edge-expansion-requirements.yml](edge-expansion-requirements.yml) |
| [Upgrade Edge](upgrade-edge.yml) | [upgrade-edge.yml](upgrade-edge.yml) | [upgrade-edge-requirements.yml](upgrade-edge-requirements.yml) |
| [Clean Control Server](clean.yml) | [clean.yml](clean.yml) | NA | 
| [Hard Remove of Apigee from a Node](apigee-node-rollback.yml) | [apigee-node-rollback.yml](apigee-node-rollback.yml) | NA |
| [Download Apigee Logs](apigee-log-config-files.yml) | [apigee-log-config-files.yml](apigee-log-config-files.yml) | NA |
| [Apigee Bash Scripts Debug Mode](apigee-opdk-debug-mode.yml) | [apigee-opdk-debug-mode.yml](apigee-opdk-debug-mode.yml) | [apigee-opdk-debug-mode-requirements.yml](apigee-opdk-debug-mode-requirements.yml) | 


