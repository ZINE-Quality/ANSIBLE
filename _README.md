# ANSIBLE
Collection of useful Ansible Playbooks
Create an inventory file and run. 

Playbook execution example: 
ansible-playbook -i inventory.txt playbook.yml --ask-become

Inventory file example:
[ALL]
Hostname ansible_host=192.168.1.45 ansible_user=username

ssh key authentication needs to be copied over prior to execution. I also like to manually ssh one time to add the server to the known hosts.
ssh-copy-id username@192.168.1.45
