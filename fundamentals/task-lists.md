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
### **resource\_name: ''**

The name you would like to use for the VM resource
{% endhint %}

{% hint style="info" %}
### **hostname: - **_**optional**_

The hostname you would like to use for the VM
{% endhint %}

{% hint style="info" %}
### **dns\_hostname: - **_**optional**_

The DNS hostname you would like to use for the VM
{% endhint %}

### **size: - **_**optional**_

The size of the instance for the VM. This will change depending on the cloud you use.

### **region: - **_**optional**_

The region you would like to use for the VM. This will change depending on the cloud you use.

### **img: - **_**optional**_

The cloud provider operating system to use. Currently, Warhorse only supports Ubuntu 20.04. This will change in the future. This will change depending on the cloud you use.

### **http\_proxy: - **_**optional**_

The HTTP proxy you would like to use with your modules. Currently, only traefik and Nginx are supported

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
