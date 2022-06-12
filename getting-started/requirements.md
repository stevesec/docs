# Requirements

### Software

To use Warhorse we need to install two different software packages Ansible and Terraform. The instructions to install this software are below.

{% tabs %}
{% tab title="Windows" %}
#### Windows

####
{% endtab %}

{% tab title="macOS" %}
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
{% endtab %}

{% tab title="Linux" %}
```bash
cd warhorse
ansible-galaxy install -r requirements.yml -p roles/
export ANSIBLE_VAULT_PASSWORD_FILE=./vault-env
```

Run the following command from the root of the warhorse repository folder to install all Ansible roles.

**Install Role dependencies**

```bash
sudo apt-get update && sudo apt-get install -y gnupg software-properties-common curl
curl -fsSL https://apt.releases.hashicorp.com/gpg | sudo apt-key add 
sudo apt-add-repository "deb [arch=amd64] https://apt.releases.hashicorp.com $(lsb_release -cs) main"
sudo apt-get update && sudo apt-get install terraform
```

Run the following commands to install Terraform with APT

**Install Terraform**

```bash
sudo apt-get update
sudo apt-get install software-properties-common -y
sudo apt-add-repository --yes --update ppa:ansible/ansible
sudo apt-get update
sudo apt-get install ansible-core -y
```

Run the following commands to install Ansible with APT

**Install Ansible**

### Domain Name <a href="#_2-cloud-provider" id="_2-cloud-provider"></a>
{% endtab %}
{% endtabs %}

### DNS

You will need to buy a domain name. For our use case, the name does not really matter. I would recommend that you only use this domain for Warhorse but it is possible to reuse your domain name. There are lots of great places to buy a domain name, one good one is [https://porkbun.com/](https://porkbun.com/)

### Cloud Provider

You will need to use a cloud provider and more importantly, you will need API keys. You will only need API keys for the services you plan to use.

<details>

<summary>AWS</summary>

API - Access Key API - Secret Key

</details>

<details>

<summary>Digital Ocean</summary>

API Key

</details>

<details>

<summary>Azure</summary>



</details>

### Secrets



### S3 (Compatible) Bucket&#x20;

To utilize backups and a Terraform state file you will need an S3 bucket. You can use any service as long as it support's the S3 protocol. Examples included [Amazon S3](https://aws.amazon.com/s3/), [Digital Ocean Spaces](https://www.digitalocean.com/products/spaces), and [Backblaze B2](https://www.backblaze.com/b2/cloud-storage.html) just to name a few.



### &#x20;<a href="#_2-cloud-provider" id="_2-cloud-provider"></a>
