# job4j_ansible
 The simple App for how to work with Ansible.Use Asimble DevOps dev tool.

### Usage
- Step 1
Install Asimble DevOps
```shell
sudo apt-get install ansible -y
```
- Step 2
clone repository and run playbook
```shell
git clone https://github.com/job4j/job4j_ansible.git
```
- Step 3
edit file playbook.yml for your needs
write your password in variable vault_ansible_become_pass

- Step 4
Push to GitHub

- Step 5
clone repository and run playbook
clone you repository to remote host
got to root project directory
and run playbook
```shell
ansible-playbook -i inventory.yml playbook.yml
```
- Step 6
If you need use private password, you can use vault
go to root folder project, create file vault.yml
or create secret.yml
```shell
ansible-vault create secrets.yml
```
write your password in variable vault_ansible_become_pass
```shell
ansible_become_pass: "your_password_for_vboxuser"
```