# Ansible manual


### Specify Inventory

The default location for inventory is a file called /etc/ansible/hosts. You can specify a different inventory file at the command line using the -i <path> option. You can also use multiple inventory files at the same time, and/or pull inventory from dynamic or cloud sources or different formats (YAML, ini, etc), as described in Working with dynamic inventory. Introduced in version 2.4, Ansible has Inventory Plugins to make this flexible and customizable.

`ansible -i ./hosts -m ping`

### Running playbook with become

`ansible-playbook ubuntu1804_redmine.yml -K`