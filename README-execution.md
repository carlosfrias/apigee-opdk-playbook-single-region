# Playbook Execution

# Playbook cli for OS Pre-Requisites
    ansible-playbook \
        install-edge-aio.yml \
        -e @~/.apigee/credentials.yml \
        -e @~/.apigee/custom-properties.yml \
        --become \
        --become-method=pbrun \
        --skip-tags=root,selinux,apigee-user,iptables,ipv6,os-common,remove-targets,restore-targets \
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

