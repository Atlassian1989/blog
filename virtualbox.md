Enable guest editions in case of virtualbox  
===========================================  
sudo rpm --import http://apt.sw.be/RPM-GPG-KEY.dag.txt   
wget http://pkgs.repoforge.org/rpmforge-release/rpmforge-release-0.5.3-1.el6.rf.x86_64.rpm  
sudo rpm -i rpmforge-release-0.5.3-1.el6.rf.*.rpm  
to verify if it worked  
sudo yum install htop  
sudo yum --enablerepo rpmforge install dkms  
sudo yum groupinstall "Development Tools"  
sudo yum install kernel-devel  
sudo yum update  
restart  
cd /media/VBOXADDITIONS_4.3.12_9373  
sudo ./VBoxLinuxAdditions.run  
  
Ref:  
http://wiki.centos.org/HowTos/Virtualization/VirtualBox/CentOSguest  
http://wiki.centos.org/AdditionalResources/Repositories/RPMForge#head-f0c3ecee3dbb407e4eed79a56ec0ae92d1398e01  

## Mounting shared folder
```sh
sudo mount -t vboxsf share /home/folder/path
```
