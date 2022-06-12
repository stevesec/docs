# Building a Configuration

The configuration for Warhorse consists of a simple Yaml file. The values in this file are used by Ansible to build Terraform and to configure our Operating system and applications.

<details>

<summary>General</summary>

### **op\_number: '123456'**

This is a unique number used to identify the engagement.

### **user\_tag: 'operator'**

name to identify the user that deployed the engagement**.**

### **ttl: '2022-12-30'**

Time to Live for the engagement year month day 2022-01-01

### **ntp\_timezone:** 'America/New\_York'

The time zone you would like to use for all VM's and log data

</details>
