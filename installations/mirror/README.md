Apigee Mirror Playbooks
=============================

These playbooks are designed to work with an Apigee mirror in preparation for performing offline
 installations of Apigee Edge Private Cloud. These playbooks perform the following functions:
 
 * Create an Apigee Mirror on a designated server.
 * Download an Apigee Mirror from a designated server
 * Upload an Apigee Mirror to a designated server
 * Install an Apigee Mirror to a designated server
 * Setup the Apigee Nginx Web server as a yum repository for Apigee Edge Private Cloud installation
 
# Assumptions

* These playbooks assume that you have configured an `ansible.cfg` that indicates the location of the 
inventory and Ansible roles.
* This playbook assumes you have invoked `ansible-galaxy install -r requirements.yml -f`
 
# Creating an Apigee Mirror
You can create an Apigee Mirror with the `create-archive.yml` playbook. You will need to indicate the 
target host that should be used to create the playbook. The target host is optimally a machine with
internet access. You indicate the target host by passing `target_host` during the invocation of this
script.

## Usage to Create an Apigee Mirror

    ansible-playbook create-archive.yml -e target_hosts=mirror
         
# Download an Apigee Mirror
Assuming you have created an Apigee OPDK mirror with the default settings and you need to download an Apigee mirror, 
then you can use the following playbook: 
 
    ansible-playbook create_download_apigee_mirror.yml -vv -b --tags=download

# Uploading and Installing an Apigee Mirror
Assuming you need to upload and install an Apigee mirror with the playbook default settings, then you can use the 
following:
   
    ansible-playbook upload_install_apigee_mirror.yml -vv -b
    
## Upload an Apigee Mirror
Assuming you have an Apigee OPDK mirror in the location set by the playbook default settings and you need to upload the
mirror to a server, then you can use the following:

    ansible-playbook upload_install_apigee_mirror.yml -vv -b --tags=upload

## Install an Apigee Mirror
Assuming you have an Apigee OPDK mirror already uploaded to the location set by the playbook default settings and you 
need to install that Apigee mirror, then you can use the following:

    ansible-playbook upload_install_apigee_mirror.yml -vv -b --tags=install
<!-- BEGIN Google Required Disclaimer -->

# Not Google Product Clause

This is not an officially supported Google product.
<!-- END Google Required Disclaimer -->
<!-- BEGIN Google How To Contribute -->
# How to Contribute

We'd love to accept your patches and contributions to this project. Please review our [guidelines](CONTRIBUTING.md).
<!-- END Google How To Contribute -->