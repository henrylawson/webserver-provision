Webserver Provision
===================
A simple Ansible project to provision my webserver.

Getting Started
===============
1. Install Ansible
1. Install VirtualBox
1. Install Vagrant
1. `vagrant plugin install vagrant-hostsupdater`
1. Install GPG
1. Install git-crypt
1. Make sure the ~/.gnupg vault is setup - linked to Dropbox
1. Unlock the encrypted files `git-crypt unlock`
1. Download the vagrant box for Ubuntu `wily-server-cloudimg-amd64-vagrant-disk1.box`
1. Add the box to vagrant `vagrant box add wily wily-server-cloudimg-amd64-vagrant-disk1.box`
1. If there are dependencies`ansible-galaxy install -r requirements.yml`
1. Run `vagrant up`

Running It
==========
1. Ensure SSH is setup, check henrylawson.net readme for details
1. `ansible-playbook playbook.yml -i hosts.gitcrypt`
