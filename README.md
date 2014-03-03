# angrycorner-ansible

Run angrycorner on your service of choice w/ RAGE. Designed for Ubuntu 12.04 x64.

## Installation

### Digital Ocean

Create a [droplet](https://www.digitalocean.com/?refcode=ebcbc179c33f) on digital ocean and note the IP Address. 

Then on your local machine, run the following.

```
git clone https://github.com/scottmotte/ansible-angrycorner.git
cd ansible-angrycorner
cp hosts.example hosts
```

Deploy using [ansible](http://www.ansibleworks.com). (install instructions for ansible are in [requirements](#requirements) below.

```
ansible-playbook playbook.yml -i hosts
```

That's it. Now ansible-angrycorner is running on its own server.

## Requirements

[Ansible](http://www.ansibleworks.com/) is required. 

### Installing Ansible on Mac

```
cd /tmp
git clone git://github.com/ansible/ansible.git
cd ./ansible
git checkout v1.4.3
sudo make install
sudo easy_install jinja2 
sudo easy_install pyyaml
sudo easy_install paramiko
```

## History

This project was originally built on [StartupBusKC](http://twitter.com/startupbuskc)'s in the year 2014. 

