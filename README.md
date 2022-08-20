# Proxmox
Information related installation, configuration, setting up,... proxmox server as VMs

# Configurar màquina virtual inicialment

##El primer que feim és actualitzar la màquina:
1. sudo apt update
2. sudo apt upgrade

##Instal·lam i engegam l'agent hoste qemu:
1. sudo apt -y install qemu-guest-agent
2. sudo systemctl enable qemu-guest-agent
3. sudo systemctl start qemu-guest-agent
4. sudo systemctl status qemu-guest-agent

