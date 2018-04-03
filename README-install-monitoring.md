# Install Apigee Monitoring Dashboard

The playbook `install-monitoring.yml` will perform an installation of the [Apigee Edge Monitoring Dashboard (Beta)](https://docs.apigee.com/private-cloud/v4.18.01/apigee-monitoring-dashboard-overview). 

## Basic Usage
We have created `ansible-galaxy` requirement file `install-monitoring-requirements.yml` that will download the roles 
used by this playbook and install them for usage according to your configuration. You can download and install the 
required roles like this: 

    ansible-galaxy install -r install-monitoring-requirements.yml -f
    
The install process will be engaged when you invoke the playbook like this:

    ansible-playbook install-monitoring.yml

## Dependencies

Dependencies are managed as described in the [README](README.md).
