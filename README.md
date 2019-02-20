# vagrant-splunk
Ubuntu 18.04x64 Bionic Beaver VM with Splunk Enterprise, 2048 GB of RAM and 2 CPUs.
Originally forked from: https://github.com/gallilama/vagrant-splunk

## Prerequisites
###### Vagrant
Vagrant 2.2.3+
Install Vagrant see https://docs.vagrantup.com/v2/installation/index.html

###### Splunk
* Download desired Splunk as Debian package (.deb)
* Place .deb in ./provision/lib
* Update the variable, SPLUNK_DEB, in Vagrantfile with correct file name
* Update the IP configuration in teh Vagrant file to your desired settings 
```config.vm.network "private_network", ip: "YOUR_IP_HERE"```

## Installation
###### Start box
```Shell
vagrant up
```

## Vagrant Controls
###### Start box
```Shell
vagrant up
```

###### SSH into box
```Shell
vagrant ssh
```
The default password is *vagrant*

###### Suspend and Resume
```Shell
vagrant suspend
vagrant resume
```

###### Tear down box
```Shell
vagrant destroy
```

#### UI Access
If using the current vagrant file it works on Virtualbox only. You will need to add a port forward for port 8000 to the network of the new VM
