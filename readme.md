# Ansible Playbooks
This repository collects ansible playbooks used for managing my own machines.  

## Basic Usage
Typically playbooks within this repo are run locally.  The command below assumes allowing the `ansible.cfg` file to use the `inventory-local` folder to define inventory(which in this repo's case is localhost)

`ansible-playbook developer.yml`


## Variables
Variables should be stored at the inventory level, e.g. `local/group_vars`, unless they are role specific, in which case they should be in that role's `vars` folder.  

## Tags
Some tags are used at the play level to describe what the tasks are doing.  They can be used to skip or include certain tasks using `--skip-tags` or `--tags` accordingly.  

Current tags in use: 

> packages
>
> prefs
>
