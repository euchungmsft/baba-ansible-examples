# Docker, Docker machine installation
Ansible playbooks to install/uninstall Docker and Docker machine

 - docker.yml : install Docker specific version (17.03.x-ce)
 - docker-latest.yml : install Docker latest
 - docker-machine.yml : install Docker machine
 - docker-compose.yml : install Docker compose specific version (1.15.0)
 - remove-all-images.yml : stops all containers, removes all containers and images 
 - remove-docker.yml : uninstall Docker 
 - remove-docker-machine.yml : install Docker machine

*Notes*
For Docker and Docker machine, installs specific version not the latest version because Rancher installation as next step. See vars section for both playbooks