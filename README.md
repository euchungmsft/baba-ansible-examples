
# baba-ansible-examples
Ansible examples

To run these examples

 1. Install Ansible at your controller 
 See http://docs.ansible.com/ansible/latest/intro_installation.html

Config Ansible hosts

    $ echo "127.0.0.1" > ~/ansible_hosts
    $ export ANSIBLE_INVENTORY=~/ansible_hosts

Configuring Ansible inventories 
http://docs.ansible.com/ansible/latest/intro_inventory.html

2. Create nodes to run the playbooks from Aliyun Portal

3. SSH key generation and deploy it to all nodes

Key generation 

    $ ssh-keygen -t rsa 

Deploying the key

    $ ssh-copy-id [account, root]@[host name]

4. Test config

    $ ansible all -m ping






