# General

{% tabs %}
{% tab title="Required" %}
{% hint style="danger" %}
### **op\_number: '123456'**

This is a unique number used to identify the engagement.
{% endhint %}

{% hint style="danger" %}
### **user\_tag: 'operator'**

name to identify the user that deployed the engagement**.**
{% endhint %}

{% hint style="danger" %}
### **ttl: '2022-12-30'**

Time to Live for the engagement year month day 2022-01-01
{% endhint %}


{% endtab %}

{% tab title="Optional" %}
{% hint style="info" %}
### **ntp\_timezone:** 'America/New\_York'

The time zone you would like to use for all VM's and log data
{% endhint %}
{% endtab %}
{% endtabs %}

#### Example

```yaml
    general:
        op_number: "123456"
        user_tag: 'operator'
        ttl: '2022-12-30' #Kill Date
        ntp_timezone: 'America/New_York' # Time Zone Link
```
