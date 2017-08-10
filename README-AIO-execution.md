# Playbook Execution

Custom properties and credentials have been included in the playbook so they do not
need to be passed in on the command line. Additionally, roles that are not suitable
for Verizon provisioned instances have been removed so that they no longer need to be
listed in --skip-tags.

# Playbook cli to update the Ansible cache
    ansible-playbook \
        install-edge-aio.yml \
        --tags=cache

# Playbook cli for OS Pre-Requisites
    ansible-playbook \
        install-edge-aio.yml \
        --become \
        --become-method=pbrun \
        --tags=os-pre-req

# Playbook cli for Apigee Pre-Requisites
    ansible-playbook \
        install-edge-aio.yml \
        --become \
        --become-method=pbrun \
        --tags=apigee-pre-req

# Playbook cli for Apigee Configuration
    ansible-playbook \
        install-edge-aio.yml \
        --become \
        --become-method=pbrun \
        --tags=apigee-config

# Playbok cli for Apigee Component installation
    ansible-playbook \
        install-edge-aio.yml \
        --become \
        --become-method=pbrun \
        --skip-tags=cache,os-pre-req,apigee-pre-req

