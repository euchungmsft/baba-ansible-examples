# Oracle installation
Oracle 12 (12.1.0.2) installation on Docker

This example automated the Oracle installation when you try to use Oracle's official release on Docker Store

https://store.docker.com/images/oracle-database-enterprise-edition

 - ora12install.yml : install Oracle
 - ora12install-check.yml : check the status to ensure the Oracle installation done
 - ora12install-clients.yml : install Oracle client
 - ora12init.yml : Initialization with a new table space and user creation
 - variables.yml : variables to apply for all 

How to run

 1. Install Docker 
 2. Update variables.yml - See the instructions in the file
 2. Make some changes on the templates, or just move on to next step with oracle defaults
 3. Run the cookbooks at sequence listed above - ora12install.yml takes some time check the status by running ora12install-check.yml

*Notes*

There's no new database creation in this example. Try to use PDB1 as SID when you create objects. See templates\oracle_client\tnsnames.ora for further details

Add "stdout_callback = debug" to your Ansible config file (~/.ansible.cfg)

[defaults]
stdout_callback = debug

