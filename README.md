# Apigee OPDK Installation of a Single Data Center

This repository contains Ansible playbooks that use roles to install Apigee Edge, Developer Portal, Baas and the 
Monitoring Dashboard. These playbooks orchestrate the usage of the roles to achieve the following:
 
## Installing Apigee Components 
| Playbook Description | Playbook Name | Playbook Role Requirements |
| --- | --- | --- |
| [Install AIO](install-edge-aio.yml) | [install-edge-aio.yml](install-edge-aio.yml) | [install-edge-aio-requirements.yml](install-edge-aio-requirements.yml) |
| [Install Edge](install-edge.yml) | [install-edge.yml](install-edge.yml) | [install-edge-requirements.yml](install-edge-requirements.yml) |
| [Install Developer Portal](install-devportal.yml) | [install-devportal.yml](install-devportal.yml) | [install-devportal-requirements.yml](install-devportal-requirements.yml) |
| [Install Baas](install-baas.yml) | [install-baas.yml](install-baas.yml) | [install-baas-requirements.yml](install-baas-requirements.yml) |
| [Install Monitoring Dashboard](install-monitoring.yml) | [install-monitoring.yml](install-monitoring.yml) | [install-monitoring-requirements.yml](install-monitoring-requirements.yml) |
| [Install Apigee Mirror](install-mirror.yml) | [install-mirror.ym](install-mirror.yml) | [install-mirror-requirements.yml](install-mirror-requirements.yml) |
| [Install Monetization](install-monetization.yml) | [install-monetization.yml](install-monetization.yml) | [install-monetization-requirements.yml](install-monetization-requirements.yml) |

## Expanding Apigee
* [Add a Data Center to a Planet](edge-expansion.yml)
* [Upgrade Edge](upgrade-edge.yml)

## Node Maintenance Tasks
* [Clean Control Server](clean.yml)
* [Hard Remove of Apigee from a Node](apigee-node-rollback.yml)
* [Download Apigee Logs](apigee-log-config-files.yml)
