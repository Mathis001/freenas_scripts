# freenas_scripts

#Create a link from this folder to /home/user/.scripts

`ln -s /path/to/freenas_scripts /home/user/.scripts`

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

