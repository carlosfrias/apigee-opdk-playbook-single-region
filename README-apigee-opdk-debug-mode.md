# Enable Debug Mode for Apigee Edge Scripts

The playbook `apigee-opdk-debug-mode.yml` will set the debug flag on all of the Edge component scripts. 
 
## Usage 
To set debug mode you invoke the playbook like this: 

    ansible-playbook apigee-opdk-debug-mode.yml -e opdk_debug_mode='on'
    
To unset debug mode you invoke the playbook like this:

    ansible-playbook apigee-opdk-debug-mode.yml -e opdk_debug_mode='off'
    
To set debug mode on the scripts for an Edge component then use the `-e component_name` variable like this:
 
    ansible-playbook apigee-opdk-debug-mode.yml -e opdk_debug_mode='on' -e component_name='message-processor'
    
    
## Dependencies

This playbook assumes that you followed the instructions for setting up [Ansible](https://github.com/carlosfrias/apigee-opdk-playbook-setup-ansible).    
Please refer to the documentation for [apigee-opdk-debug-mode](https://github.com/carlosfrias/apigee-opdk-debug-mode). 
