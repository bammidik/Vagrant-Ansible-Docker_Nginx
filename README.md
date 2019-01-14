# Vagrant-Ansible-Docker_Nginx

Vagrant using ansible provisioner.
Vagrant let's us run custom provisioners such as Puppet, Chef, Ansible, Salt, or Shell.
In this case we are using ansile as a provisioner.
The ansible provisioner including 2 roles
  1. The first role install and start/enable docker service on the guest machine
 2. The second role crates a nginx docker container using library/alpine:latest as base image
The nginx process with in the continer run as nobody user and serves a sample "Hello World" page

Note: This vagrant  file creates an addional network interface  in bridge mode, please update the vagrant file with interface name matching your host machine interface and a ip address from your host network range.

Once vagrant provisioing is completed, you can access the sample web page on post 80 of that ip.
