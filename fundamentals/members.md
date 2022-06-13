# DNS

{% tabs %}
{% tab title="Required" %}
{% hint style="danger" %}
### **provider: 'digitalocean'**

The cloud provider you want to use for DNS.
{% endhint %}

{% hint style="danger" %}
### **op\_tld: 'operation.com'**

The top-level domain name for DNS
{% endhint %}

{% hint style="danger" %}
### **op\_domain\_name: 'op.operation.com'**

The operation subdomain you want to use for DNS
{% endhint %}
{% endtab %}

{% tab title="Optional" %}

{% endtab %}
{% endtabs %}

### **Example**

```
  dns:
    provider: "digitalocean"
    op_tld: 'operation.com'
    op_domain_name: '123456.operation.com'
```
