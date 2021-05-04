# rpi_setups
Rasspbery Pi automated setups through Ansible
Author Pawel Golawski <pawel.golawski@2com.pl>

## Contents
This repository contains Ansible scripts for following tasks I do on regular basics
- [x] playbooks/update.yml - this is ```sudo apt upgrade``` with reboot if neccesary
- [x] playbooks/sync_profiles.yml - this is syncing dot "." main files as .profile and a few more with running node
- [x] playbook/nano_highlighters.yaml - it copies .nanorc common syntax highlighters into "workstations" nodes
- [ ] TBD

Before running it please create valid inventory file - see example in inventory_example.ini

Example of using specific playbook

```bash
ansible-playbook -i my_inventory_file.ini playbooks/update.yml
```

## My future plans
None at the moment
