# Drupal 7 EC2 + Ansible

## Notes

* Requires Ansible 1.9x
* We're using [ec2.py](http://docs.ansible.com/ansible/intro_dynamic_inventory.html#example-aws-ec2-external-inventory-script) for dynamic inventory
* Requires boto + aws credentials


## Installation

* Clone this repo to a local folder
* Install Ansible roles
```
sudo ansible-galaxy install -r requirements.yml --force
```
* Copy `my-vars.default.yml` to `my-vars.yml`
* Configure the variables in my-vars.yml


## Usage
```
ansible-playbook main.yml -K
```
