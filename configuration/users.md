# Users



**- username: REQUIRED**

This is the name you would like to use for a user account

**name: REQUIRED**

This is the username that will be used on your VM's

**authorized\_keys: REQUIRED**

This is the public SSH key to use for the user. You can put a file path of a github url.

**shell: REQUIRED**

This is the shell to use for the user. Default shell is ZSH

**Example**

```
users:
    - username: operator
        name: operator
        authorized_keys:
        - "{{ lookup('file', '/home/operator/.ssh/id_rsa.pub') }}"
        shell: '/usr/bin/zsh'
```
