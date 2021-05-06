# rpi_setups
Rasspbery Pi automated setups through Ansible.

Author Pawel Golawski <pawel.golawski@2com.pl>

## Contents
This repository contains Ansible scripts for following tasks I do on regular basics
* ```playbooks/update.yml``` - this is ```sudo apt upgrade``` with reboot if neccesary for ```[all]``` nodes
* ```playbooks/sync_profiles.yml``` - this is syncing dot ```.``` main files as ```.profile``` and a few more on ```[all]``` nodes with 1st node in  inventory file
* ```playbook/nano_highlighters.yaml``` - it copies ```*.nanorc``` common syntax highlighters into ```[workstations]``` nodes


## Usage
Before running it please create valid inventory file - see example in ```inventory_example.ini```

Example of using specific playbook

```bash
ansible-playbook -i my_inventory_file.ini playbooks/update.yml
```

## My future plans for playbooks (TODO)

- [ ] ```sync_profiles.yml``` - to copy whatever ```id_*``` files are in ```.ssh``` directory
- [ ] ___all___ - to make it resilent if the original files are not found (like ```.backup.sh```)

[//]: # (None at the moment)
