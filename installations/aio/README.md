# Apigee AIO Installer
This script will install the `aio` profile of the Edge installation. 

## Usage: 
This is an Ansible script and require Ansible. Please follow the usage instructions below:

### Setup 
This playbook sets creates the folder structure to store Ansible artifacts and generates 
configuration files. Expects you to provide the address to the node for the installation. 

    ansible-playbook setup.yml
    
### Dependencies
Use `ansible-galaxy` to download and install Ansible roles. This is best to perform after [Setup]
above. 
    
    ansible-galaxy install -r requirements -f
    
### Installer
This playbook completes the installation of the `aio` instances of Edge.

    
    ansible-playbook install.yml 

