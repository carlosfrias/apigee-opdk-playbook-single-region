# Playbook Execution

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

