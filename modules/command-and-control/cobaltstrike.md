# Cobaltstrike

```
cobaltstrike:
        enabled: true
        dir: "/opt/docker/cobaltstrike"
        dns_over_https: true
        auth_header_name: "cdnauth"
        auth_header_value: "value"
        password: "password"
        key: "0000-00-0000-0000"
        socks_ports:
        - 9201
        - 9202
        - 9203
        profile: malleable.profile
        cdn:
        - name: "azure"
          provider: "azure"
          hostname: "uniquename"
          redirect_url: "azure.microsoft.com"
```
