# Install the AIO profile of Apigee Edge

The playbook `install-edge-aio.yml` will perform an installation of AIO version of Apigee Edge. Version 4.16.xx through 4.18.01 can be installed
from this playbook. 

## Basic Usage
We have created `ansible-galaxy` requirement file `install-monitoring-requirements.yml` that will download the roles 
used by this playbook and install them for usage according to your configuration. You can download and install the 
required roles like this: 

    ansible-galaxy install -r install-edge-aio-requirements.yml -f
    
The install process will be engaged when you invoke the playbook like this:

    ansible-playbook install-edge-aio.yml

## Dependencies

Dependencies are managed as described in the [README](README.md).

## Inventory

Configure the [inventory](https://github.com/carlosfrias/apigee-opdk-playbook-setup-ansible#inventory-file-semantics)
 
