# Proxmox
Information related installation, configuration, setting up,... proxmox server as VMs

# Configurar màquina virtual inicialment

## Actualitzam la màquina:
* sudo apt update
* sudo apt upgrade

## Instal·lam i engegam l'agent hoste qemu:
* sudo apt -y install qemu-guest-agent
* sudo systemctl enable qemu-guest-agent
* sudo systemctl start qemu-guest-agent
* sudo systemctl status qemu-guest-agent

## Eliminam les claus ssh i en refeim de noves
* sudo rm /etc/ssh/ssh_host_*
* sudo dpkg-reconfigure openssh-server

## Esborram la clau machine-id i l'enllaçam amb la corresponent
* sudo truncate -s 0 /etc/machine-id
* sudo ln -s /etc/machine-id /var/lib/dbus/machine-id

## Canviam hostname pel que li toca
* sudo nano /etc/hostname 
* sudo nano /etc/hosts 
