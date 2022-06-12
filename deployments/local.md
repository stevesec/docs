# Local

### Clone Repo and Requirements

```bash
git clone https://github.com/warhorse/warhorse
cd warhorse
ansible-galaxy install -r requirements.yml -p roles/
export ANSIBLE_VAULT_PASSWORD_FILE=./vault-env
```

{% content-ref url="../configuration/building-a-configuration.md" %}
[building-a-configuration.md](../configuration/building-a-configuration.md)
{% endcontent-ref %}

### Generate Files

```
ansible-playbook generate.yml
```

### Deploy

```
ansible-playbook deploy.yml
```

### Destroy

```
ansible-playbook destroy.yml
```
