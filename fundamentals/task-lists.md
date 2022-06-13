# VM

{% hint style="danger" %}
### - **name: - 'teamserver'**

This is the name you would like to use for the Virtual Machine
{% endhint %}

{% hint style="danger" %}
### **provider: - 'digitalocean'**

The cloud provider you want to use for Virtual Machine.
{% endhint %}

{% hint style="info" %}
### **resource\_name: '**operator-0000-01-teamserver'

The name you would like to use for the VM resource
{% endhint %}

{% hint style="info" %}
### **hostname: '**123456-teamserver'

The hostname you would like to use for the VM
{% endhint %}

{% hint style="info" %}
### **dns\_hostname: '**teamserver'

The DNS hostname you would like to use for the VM
{% endhint %}

{% hint style="info" %}
### **size: '**s-2vcpu-4gb'

The size of the instance for the VM. This will change depending on the cloud you use.
{% endhint %}

{% hint style="info" %}
### **region: '**nyc1'

The region you would like to use for the VM. This will change depending on the cloud you use.
{% endhint %}

{% hint style="info" %}
### **img: '**ubuntu-20-04-x64'

The cloud provider operating system to use. Currently, Warhorse only supports Ubuntu 20.04. This may change in the future. The name will change depending on the cloud you use.
{% endhint %}

{% hint style="info" %}
### **http\_proxy: '**traefik'

The HTTP proxy you would like to use with your modules. Currently, only traefik and Nginx are supported
{% endhint %}

### **Example**

```
  vm:
    - name: "teamserver"
        provider: "digitalocean"
        resource_name: "operator-0000-01-teamserver"
        hostname: "123456-teamserver" optional
        dns_hostname: "teamserver" optional
        size: "s-2vcpu-4gb" optional
        region: "nyc1" optional
        img: "ubuntu-20-04-x64" optional
        http_proxy: "traefik" # nginx,caddy
```
