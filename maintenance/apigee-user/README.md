# Simplified Apigee User Setup
This script will setup the `apigee` user on the apigee instances.

## Usage: 
This is an Ansible script and require Ansible. Two installation mechanisms are available:

### Quick Start
This quick start will attempt to download Ansible roles and run `update-apigee-user.yml` 

    ansible-pull -U https://github.com/carlosfrias/apigee-opdk-playbook-installation-single-region maintenance/apigee-user/setup.yml
    
### Manual Setup
Assuming the quick start has an issue you can fall back to a semi-automated setup:

    ansible-galaxy install -r requirements -f
    ansible-playbook update-apigee-user.yml -e target_hosts=<IP address to host>
        