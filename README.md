# manpi-config
Ansible Playbooks for configuration of Raspberry Pi Manjaro-KDE


## Requirements

Ansible (>= 2.8) needs to be installed. On Manjaro, use the following command:
pacman -S ansible

The vault.yml (not included) needs to be created and should include the following variables:
- vnc_pass: 

## Included Files

This project contains the following files:
- adhoc                 -> Adhoc script for initial setup (passwordless sudo on localhost)
- ansible.cfg           -> contain ansible config for executing against the local host
- config-avahi.yml      -> Playbook to install and configure Bonjour for local dynamic dns
- config-x11vnc.yml     -> Playbook to install and configure VNC server
- group_vars            -> group_vars for the project (requires a vault.yml file -not in this repo-)
- install_packages.yml  -> Playbook to install and configure additional packages. Currently only docker
- install-pykms.yml     -> Playbook to install and configure py-kms
- inventory             -> Inventory file for this project (only containing localhost)
- README.md             -> This file
- template              -> directory containing jinja2 templates
