# Showcase vagrant

## Requirement 

### Vagrant installation

- Install vagrant
- Install virtual box
- Download vm box (recommended: ubunntu/bionic64)
- Install docker compose plugin "vagrant plugin install vagrant-docker-compose"

### Aditional Notes 

- Virtual machine box : ubuntu/bionic64 -> ubuntu 18.04 
- Modify memory value in Vagrantfile depending on host machine ressources 
- Modify ip address for the private network in Vagrantfile if it's neccesary 

## Docker containers

- jenkins
- gitlab (add to docker list in Vagrantfile)
- nexus
- portainer
- wireguard server 