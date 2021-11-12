# Automatic tools installation on work laptop
The goal of this project is to create an automation via Ansible in order to configure and install basic tools in a work notebook

## Dependecies ##
- ansible >= v2.11.6
- ansible-galaxy >= v2.11.6

## Installing External Roles ##

1 - To install external roles run the role_update.sh script which will download all roles via Ansible Galaxy.
```bash
./external/setup/role_update.sh     
```

## Running the Playbook ##

2 - To run the playbook run the following command.
```bash
ansible-playbook -i inventory/host plays/playbook .yml    
```
 
## References ##
https://galaxy.ansible.com/

https://githubmemory.com/repo/agowa338/ansible-best-practises