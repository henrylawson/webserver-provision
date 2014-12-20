Webserver Provision
===================
A simple Ansible project to provision my webserver.

Getting Started
===============
1. Install Ansible
1. Install Virtual Box
1. Install Vagrant
1. Install git-crypt
1. Make sure the ~/.gnupg vault is setup - linked to Dropbox
1. Unlock the encrypted files `git-crypt unlock`
1. Download the vagrant box for Ubuntu - `utopic-server-cloudimg-amd64-vagrant-disk1.box`
1. Add the box to vagrant `vagrant box add utopic utopic-server-cloudimg-amd64-vagrant-disk1.box`
1. Run `vagrant up`

Working
=======
1. Get the hosts IP `ping vagrant-webserver`
1. Setup the `sudo vi /etc/hosts` file to have the entries `XXX.XXX.X.XX foinq.com`
1. Ensure it is working by `ping foinq.com`
1. View website in browser
1. Make changes run `vagrant provision`
1. Destroy changes run `vagrant destroy`
1. To ensure files are encrypted, append the "gitcrypt" extension on the end as defined in .gitattributes