# Ansible Playbooks
This repository collects ansible playbooks used for managing my own machines.  

## Basic Usage
Typically playbooks within this repo are run locally.  Use the `local` folder as an inventory source, in combination with a playbook at the top level, e.g.
`ansible-playbook -i local developer.yml`

## Variables
Variables should be stored at the inventory level, e.g. `local/group_vars`, unless they are role specific, in which case they should be in that role's `vars` folder.  