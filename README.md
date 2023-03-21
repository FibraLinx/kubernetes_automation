# Procedure to automatically deploy a kubernetes cluster using vagrant and ansible

## Prerequisites
Local ubuntu machine with installed:
- vagrant
- virtualbox
- ansible

## Setup on local host

1. Create a project directory
- `mkdir -p ~/vagrant/kubernetes`

2. Create key-pair (named vagrant_key)
- `ssh-keygen -b 4096`

3. Run VMs
- `vagrant up`

4. Run ansible playbook
- `ansible-playbook -i hosts install-k8s.yml`
