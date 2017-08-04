# Playbook Execution

# Playbook cli to update the Ansible cache
    ansible-playbook \
            install-edge-aio.yml \
            -e @~/.apigee/credentials.yml \
            --tags=cache

# Playbook cli for OS Pre-Requisites
    ansible-playbook \
        install-edge-aio.yml \
        -e @~/.apigee/credentials.yml \
        -e @~/.apigee/custom-properties.yml \
        --become \
        --become-method=pbrun \
        --skip-tags=root,selinux,iptables,ipv6,remove-targets,restore-targets,pg-swap-file \
        --tags=os-pre-req

# Playbook cli for Apigee Pre-Requisites
    ansible-playbook \
        install-edge-aio.yml \
        -e @~/.apigee/credentials.yml \
        -e @~/.apigee/custom-properties.yml \
        --become \
        --become-method=pbrun \
        --skip-tags=remote-targets,restore-targets \
        --tags=apigee-pre-req

# Playbok cli for Apigee component installation
    ansible-playbook \
        install-edge-aio.yml \
        -e @~/.apigee/credentials.yml \
        -e @~/.apigee/custom-properties.yml \
        --become \
        --become-method=pbrun \
        --skip-tags=cache,os-pre-req,apigee-pre-req

