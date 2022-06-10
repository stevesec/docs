# macOS

**Install Ansible**

Run the following command to install Ansible with brew.

```bash
brew install ansible
```

**Install Terraform**

Run the following command to install Terraform with brew.

```bash
brew install terraform
```

**Install Role Dependencies**

Run the following command from the root of the warhorse repository folder to install all Ansible roles.

```bash
cd warhorse
ansible-galaxy install -r requirements.yml -p roles/
export ANSIBLE_VAULT_PASSWORD_FILE=./vault-env
```
