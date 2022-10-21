# Ansible Laptop Setup (Pop!_OS 22.04 LTS)

Ansible playbook designed to automate laptop setup.

## Pre-requisites 

Install python and pip
```bash
sudo apt install python3 python3-pip
```

Install ansible
```bash
sudo pip3 install ansible psutil
```

Clone this repository and cd into this project folder
```bash
git clone https://github.com/helioha/ansible-laptop-setup.git && cd ansible-laptop-setup
```

Install ansible requirements
```bash
ansible-galaxy install -r requirements.yml -p ./roles
```

## Running the playbook

To run the playbook
```bash
ansible-playbook main.yml --ask-become-pass
```

To run only certain tags in the playbook
```bash
ansible-playbook main.yml --ask-become-pass --tags "tag1,tag2,tag3"
```
