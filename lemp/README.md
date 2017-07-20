# LEMP + Wordpress
NGINX, PHP, Wordpress installation

1. Make some changes to 'templates/lemp/nginx.conf with' your own configs

2. Make some changes to 'templates/wordp/wp-config.php' with your own configs from RDS

3. Run the playbooks

Installing lemp to your instances

    $ ansible-playbook --verbose -l [host ip/alias as target] lemp.yml

Installing wordpress to your instances

    $ ansible-playbook --verbose -l [host ip/alias as target] wordp.yml
