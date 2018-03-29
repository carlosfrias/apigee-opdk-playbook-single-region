# Upgrading Apigee Edge

The playbook `upgrade-edge.yml` will perform an upgrade of Apigee Edge. Edge 4.16.xx is supported for upgrade
through Edge 4.18.01. 

## Usage 
The upgrade process will be engaged when you invoke the playbook like this: 

    ansible-playbook update-edge.yml
     
Please note that the variables below need to be set either upon invocation of the playbook or by updating your custom-properties.yml 

## Variables Used
| Variable Name | Value | Description |
| --- | --- | --- |
| opdk_version | 4.18.01 | This indicates the target opdk version to be installed. This is also set during a clean installation of OPDK. | 
| upgrade_from_opdk_version | 4.16.01, 4.16.05, 4.16.09, 4.17.01, 4.17.05, 4.17.09 | This is the version of opdk that you would be upgrading from |

 