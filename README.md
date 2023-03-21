# Procedure to automatically deploy a kubernetes cluster using vagrant and ansible

## Prerequisites
Local ubuntu machine with installed:
- vagrant
- virtualbox
- ansible

## Setup on local host

1. Clone this git repo to your local system

2. Create key-pair (named vagrant_key)
- `ssh-keygen -b 4096`

3. CD to the git folder and start vagrant VMs
- `vagrant up`

4. Run ansible playbook
- `ansible-playbook -i hosts install-k8s.yml`
