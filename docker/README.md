# Docker, Docker machine installation
Ansible playbooks to install/uninstall Docker and Docker machine

 - docker.yml : install Docker 
 - docker-machine.yml : install Docker machine
 - remove-all-images.yml : stops all containers, removes all containers and images 
 - remove-docker.yml : uninstall Docker 
 - remove-docker-machine.yml : install Docker machine

*Notes*
For Docker and Docker machine, installs specific version not the latest version because Rancher installation as next step. See vars section for both playbooks