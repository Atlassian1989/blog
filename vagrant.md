# Beginners Guide to Using Vagrant

## Software Versions used in tutorial
```
Vagrant 1.6.3
VirtualBox 4.3.12
```

## Installation
#### Install vagrant 
http://www.vagrantup.com/downloads.html
```sh
vagrant -v (should return Vagrant x.x.x)
# all available command options
vagrant help
```

#### For vagrant ssh to work in windows
* Install git
* update %PATH% with C:\Git\bin (It contains sh.exe)

#### Add Boxes 
```sh
# Add boxes to local machines (can be resused in multiple projects)
vagrant box add centos-65-x64 http://puppet-vagrant-boxes.puppetlabs.com/centos-65-x64-virtualbox-puppet.box
# Vagrant box location (added using vagrant box add):
# Mac/Linux
~/.vagrant.d/boxes
```

#### General flow
```sh
# List all boxes
vagrant box list
centos-63-x64    (virtualbox, 0)
centos-65-x64    (virtualbox, 0)
ubuntu-12.04-x64 (virtualbox, 0)

vagrant init centos-65-x64
vagrant up
vagrant ssh
vagrant halt
vagrnat destroy
```

#### Useful commands
```sh
vagrant init
vagrant up
vagrant ssh
vagrant halt
vagrant destroy
```

#### Reference:
1. http://docs.vagrantup.com/v2/getting-started/boxes.html
2. http://blog.smalleycreative.com/tutorials/setup-a-django-vm-with-vagrant-virtualbox-and-chef/
3. https://speakerdeck.com/lewg/consistent-local-development-with-vagrant-and-chef
4. http://nefariousdesigns.co.uk/vagrant-virtualised-dev-environments.html


