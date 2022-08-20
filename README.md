# Proxmox
Information related installation, configuration, setting up,... proxmox server as VMs

# Configurar màquina virtual inicialment

## Actualitzar la màquina:
1. sudo apt update
2. sudo apt upgrade

## Instal·lam i engegam l'agent hoste qemu:
1. sudo apt -y install qemu-guest-agent
2. sudo systemctl enable qemu-guest-agent
3. sudo systemctl start qemu-guest-agent
4. sudo systemctl status qemu-guest-agent

## Eliminar les claus ssh i en refeim de noves
sudo rm /etc/ssh/ssh_host_*

sudo dpkg-reconfigure openssh-server


## Esborrar la clau machine-id i enllaçar-la amb la corresponent
sudo truncate -s 0 /etc/machine-id
sudo ln -s /etc/machine-id /var/lib/dbus/machine-id

## Canviar hostname pel que li toca
sudo nano /etc/hostname 
sudo nano /etc/hosts 
