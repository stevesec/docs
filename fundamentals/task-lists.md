# VM

**- name: - Virtual Machine Name **_**REQUIRED**_

This is the name you would like to use for the Virtual Machine

**provider: - Cloud provider to use **_**REQUIRED**_

The cloud provider you want to use for Virtual Machine.

**resource\_name: - **_**optional**_

The name you would like to use for the VM resource

**hostname: - **_**optional**_

The hostname you would like to use for the VM

**dns\_hostname: - **_**optional**_

The DNS hostname you would like to use for the VM

**size: - **_**optional**_

The size of the instance for the VM. This will change depending on the cloud you use.

**region: - **_**optional**_

The region you would like to use for the VM. This will change depending on the cloud you use.

**img: - **_**optional**_

The cloud provider operating system to use. Currently, Warhorse only supports Ubuntu 20.04. This will change in the future. This will change depending on the cloud you use.

**http\_proxy: - **_**optional**_

The HTTP proxy you would like to use with your modules. Currently, only traefik and Nginx are supported

**Example**

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
