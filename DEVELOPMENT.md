 - Installing virtualbox for Ubuntu 20.04
 - 

## Installing virtualbox for Ubuntu 20.04
Download virtualbox in order to run this on Ubuntu 20.04 LTS. This is the only OS this is developed and tested on, so there may be outliers on other systems at the moment.

https://phoenixnap.com/kb/install-virtualbox-on-ubuntu
##### Test (skip and only do next if running virtualbox in production)
```bash
sudo apt-get update
sudo apt-get install virtualbox
sudo apt-get install virtualbox—ext–pack
```
##### Production (not Test)

```bash
sudo apt-get install software–properties–common
wget –q https://www.virtualbox.org/download/oracle_vbox_2016.asc -O- | sudo apt-key add -
wget -q https://www.virtualbox.org/download/oracle_vbox.asc -O- | sudo apt-key add –
# Add virtualbox reository on Ubu
sudo add-apt-repository "deb http://download.virtualbox.org/virtualbox/debian bionic contrib"
# Install latest version of Virtualbox
sudo apt-get update
sudo apt-get install virtualbox–6.0
sudo apt-get install virtualbox–5.2
wget https://download.virtualbox.org/virtualbox/6.0.8/Oracle_VM_VirtualBox_Extension_Pack-6.0.8.vbox-extpack
sudo VBoxManage extpack install Oracle_VM_VirtualBox_Extension_Pack-6.0.8.vbox-extpack
```