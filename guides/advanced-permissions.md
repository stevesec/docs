# Linux

**Install Ansible**

Run the following commands to install Ansible with APT

```
sudo apt-get update
sudo apt-get install software-properties-common -y
sudo apt-add-repository --yes --update ppa:ansible/ansible
sudo apt-get update
sudo apt-get install ansible-core -y
```

**Install Terraform**

Run the following commands to install Terraform with APT

```
sudo apt-get update && sudo apt-get install -y gnupg software-properties-common curl
curl -fsSL https://apt.releases.hashicorp.com/gpg | sudo apt-key add 
sudo apt-add-repository "deb [arch=amd64] https://apt.releases.hashicorp.com $(lsb_release -cs) main"
sudo apt-get update && sudo apt-get install terraform
```

**Install Role dependencies**

Run the following command from the root of the warhorse repository folder to install all Ansible roles.

```
cd warhorse
ansible-galaxy install -r requirements.yml -p roles/
export ANSIBLE_VAULT_PASSWORD_FILE=./vault-env
```
