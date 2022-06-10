# General

### **op\_number: '123456'**

{% hint style="info" %}
This is a unique number used to identify the engagement.
{% endhint %}

### **user\_tag: 'operator'**

{% hint style="info" %}
name to identify the user that deployed the engagement**.**
{% endhint %}

### **ttl: '2022-12-30'**

{% hint style="info" %}
Time to Live for the engagement year month day 2022-01-01
{% endhint %}

### **ntp\_timezone:** 'America/New\_York'

{% hint style="info" %}
The time zone you would like to use for all VM's and log data
{% endhint %}

#### Configuration Example

```yaml
    general:
        op_number: "123456"
        user_tag: 'operator'
        ttl: '2022-12-30' #Kill Date
        ntp_timezone: 'America/New_York' # Time Zone Link
```
