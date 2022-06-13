# DNS

**provider: Cloud provider to use**

The cloud provider you want to use for DNS.

**op\_tld: The operation top-level domain**

The top-level domain name for DNS

**op\_domain\_name: The operation sub domain**

The operation subdomain you want to use for DNS

**Example**

```
  dns:
    provider: "digitalocean"
    op_tld: 'operation.com'
    op_domain_name: '123456.operation.com'
```
