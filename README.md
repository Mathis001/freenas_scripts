# freenas_scripts

### Clone repo

`sudo git clone https://github.com/Mathis001/freenas_scripts.git ~/Documents/freenas_scripts`

### Create `.scripts` folder in your home directory

`mkdir ~/.scripts`

### Create a link from this folder to `~/.scripts`

`ln -s ~/Documents/freenas_scripts/* ~/.scripts`

### Create `.bashrc` entry to look in the new scripts folder

`echo 'export PATH="$HOME/.scripts:$PATH"' >> ~/.bashrc`

# Requirements

### Install sshpass and except

`sudo apt install sshpass except`

# Run the commands from anywhere

Commands can be run without arguments for help text

## ipmi

### Connect to ipmi

`ipmi activate <ip address>`

### Reset ipmi (bmc reset cold)

`ipmi reset <ip address>`

### ipmi info

`ipmi info <ip address>`

## sysver

### Connect to remote TrueNAS  to verify system

`sysver <model> <ip address>`

Where model is either z, x, or m.

## xipmi

### Set ipmi IP addresses for remote X-series Controller (assuming cable loopback)

`xipmi <controller IP> <IPMI Netmask> <IPMI Address> <IPMI Gateway>`

