# Rancher installation & configuration
Ansible playbooks to install and config Rancher on top of Docker

 - rancher-single.yml : Rancher installation without HA, internal DB (no persistency)
 - rancher-single-extdb.yml : Rancher installation without HA, external DB (RDS, with persistency)
 - addhost.yml : run every nodes to join the Rancher cluster after Docker installation done

*Notes*

 - For rancher-single-extdb.yml, database profile where to Rancher   
   configs are stored to be defined in the playbook. See vars section
   
 - For addhost.yml, configs with ip addresses and registration token has
   to be changed. Both of internet and intranet ip addresses are fine
   but be careful with Security Group/VPC settings. Registration token
   can be found from 'add host' menu on the Rancher UI