# acit4640-lab7


### create ssh key
```ssh-keygen -t ed25519 -f ~/.ssh/aws```
* Generates a new SSH key pair named aws in your ~/.ssh directory.
* -t ed25519 specifies the secure Ed25519

### run script to import and delete key
```./import_lab_key ~/.ssh/aws.pub```

### terraform
```terraform init```
* Downloads provider plugins and initializes the working directory

```terraform fmt```
* formats Terraform files for readability

```terraform validate```
* Checks syntax and configuration are valid

```terraform plan```
* Shows what resources Terraform will create, modify, or destroy

```terraform apply```
* Creates the infrastructure as defined in the Terraform files

### ansible
```ansible -i inventory/hosts.yml all -m ansible.builtin.ping```
* Uses the ping module to verify SSH connectivity to all inventory hosts
* -i for inventory file to specify which inventory file to use
* -m for module for which ansible module to use like ping

```ansible-playbook -i inventory/hosts.yml playbook.yml --syntax-check```
* Validates the playbook syntax

```ansible-playbook -i inventory/hosts.yml playbook.yml```
* Applies the playbook tasks to all hosts in the inventory

<img width="2856" height="1034" alt="image" src="https://github.com/user-attachments/assets/d8f23c16-bef1-4ab4-8bdd-10c3634f2136" />
