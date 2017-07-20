# baba-ansible-examples
Ansible examples

- NGINX + PHP + Wordpress installation

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

- NGINX + PHP + Wordpress installation

1. Make some changes to templates/lemp/nginx.conf with your own config

2. Make some changes to templates/wordp/wp-config.php with your own config from RDS

3. Run the playbooks

Installing lemp to your instances

$ ansible-playbook --verbose -l eg-jp-ecs-001 wordp.yml

Installing wordpress to your instances

$ ansible-playbook --verbose -l eg-jp-ecs-001 wordp.yml