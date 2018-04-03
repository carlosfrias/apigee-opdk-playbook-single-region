# Install Apigee Devportal

The playbook `install-devportal.yml` will perform an installation of Apigee Devportal. 

## Basic Usage
We have created `ansible-galaxy` requirement file `install-monitoring-requirements.yml` that will download the roles 
used by this playbook and install them for usage according to your configuration. You can download and install the 
required roles like this: 

    ansible-galaxy install -r install-devportal-requirements.yml -f
    
The install process will be engaged when you invoke the playbook like this:

    ansible-playbook install-devportal.yml

## Dependencies

Dependencies are managed as described in the [README](README.md).
