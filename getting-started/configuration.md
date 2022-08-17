# Configuration

We need to build a configuration to deploy our infrastructure. While this is the heart of how Warhorse can be customized the following is a very simple configuration to use for your first deployment.

```yaml
warhorse:
  general:
    op_number: "0000"
    user_tag: 'user1'
    ttl: '2022-07-30' #Kill Date
    ntp_timezone: 'America/New_York' # Time Zone Link
    vault_key: 'password'
  dns:
    provider: "digitalocean"
    op_tld: 'CHNAGEME.com' # Resource Domain
    op_domain_name: '0000.CHANGEME.dev'
  vm:
    - name: "host1"
      provider: "digitalocean"
      http_proxy: "nginx"
      firewall: 
        enabled: true
      backup: 
        enabled: false
        archive_zip: false
  terraform:
    digitalocean_token: ""
  users:
    - username: 'hacker'
      name: 'hacker'
      authorized_keys:
      - "{{ lookup('file', '~/.ssh/hackerops.pub') }}"
      shell: '/usr/bin/zsh'
```

{% content-ref url="../configuration/building-a-configuration.md" %}
[building-a-configuration.md](../configuration/building-a-configuration.md)
{% endcontent-ref %}
