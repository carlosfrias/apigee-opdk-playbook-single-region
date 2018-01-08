# Apigee OPDK Installation of a Single Data Center

This repository contains Ansible playbooks that use roles to install Apigee Edge, Developer Portal, Baas and the 
Monitoring Dashboard. These playbooks orchestrate the usage of the roles to achieve the following:
 
* [AIO Installation](install-edge-aio.yml): Please obtain role dependencies with `ansible-galaxy install -r install-edge-aio-requirements.yml`



## Ansible Roles that support Apigee OPDK Installation

The following ansible roles will be installed with the requirements.yml file:

* [opdk-setup-apigee-user](https://github.com/carlosfrias/apigee-opdk-setup-apigee-user)
* [opdk-setup-os-common](https://github.com/carlosfrias/apigee-opdk-setup-os-common)
* [opdk-setup-os-ds](https://github.com/carlosfrias/apigee-opdk-setup-os-ds)
* [opdk-setup-os-minimum](https://github.com/carlosfrias/apigee-opdk-setup-os-minimum)
* [opdk-setup-default-settings](https://github.com/carlosfrias/apigee-opdk-setup-default-settings)
* [opdk-time-sync](https://github.com/carlosfrias/apigee-opdk-time-sync)
* [opdk-setup-openjdk](https://github.com/carlosfrias/apigee-opdk-setup-openjdk)
* [opdk-setup-bootstrap](https://github.com/carlosfrias/apigee-opdk-setup-bootstrap)
* [opdk-setup-silent-installation-config](https://github.com/carlosfrias/apigee-opdk-setup-silent-installation-config)
* [opdk-setup-component](https://github.com/carlosfrias/apigee-opdk-setup-component)
* [opdk-setup-component-installer](https://github.com/carlosfrias/apigee-opdk-setup-component-installer)
* [opdk-setup-selinux-disable](https://github.com/carlosfrias/apigee-opdk-setup-selinux-disable)
* [opdk-shutdown-iptables](https://github.com/carlosfrias/apigee-opdk-shutdown-iptables)
* [opdk-setup-org-config](https://github.com/carlosfrias/apigee-opdk-setup-org-config)
* [opdk-setup-org](https://github.com/carlosfrias/apigee-opdk-setup-org)
* [opdk-setup-validate](https://github.com/carlosfrias/apigee-opdk-setup-validate)
* [opdk-setup-validate-cleanup](https://github.com/carlosfrias/apigee-opdk-setup-validate-cleanup)
* [opdk-setup-apigee-log-files](https://github.com/carlosfrias/apigee-opdk-setup-apigee-log-files)
* [fetch-files](https://github.com/carlosfrias/apigee-fetch-files)

