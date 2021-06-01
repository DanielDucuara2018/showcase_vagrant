# Notes

Increase PEER environment variable in order to add new peers to wireguard server:
- Modify PEER env variable located in /docker/wireguard_server/.env file or in /docker/wireguard_server/docker-compose.yml file of the current folder project
- Reload vagrant machine from the terminal using: vagrant reload

Get peer.conf file:
- Create a sftp access using MobaXterm or fileZilla: using the ip address 127.0.0.1, port 2222, user vagrant and private key located in  .vagrant/machines/default/virtualbox/private_key
- Copy the peer.conf file located in config /home/vagrant/docker-data/wireguard/config/peer# in the host machine 

Show peer QR code:
- SSH access to linux vagrant machine from terminal using: vagrant ssh
- Execute: docker exec -it wireguard /app/show-peer "PEER_NUMBER"

Show peer list status:   
- SSH access to linux vagrant machine: vagrant ssh  
- Execute: docker exec -it wireguard wg
