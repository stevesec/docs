# Terraform

{% tabs %}
{% tab title="First Tab" %}
{% hint style="info" %}
### **state\_bucket\_enabled: 'true'**

This will enable the terraform state bucket in an S3 bucket.
{% endhint %}

{% hint style="info" %}
### **state\_bucket\_name: 'mybucket'**

The name of the S3 bucket
{% endhint %}
{% endtab %}

{% tab title="Second Tab" %}

{% endtab %}
{% endtabs %}

**state\_bucket\_key: REQUIRED**

This is the path to the state file in the S3 bucket.

**state\_bucket\_region: REQUIRED**

This is the region used for the S3 bucket.

**state\_bucket\_endpoint: REQUIRED**

This is the URL used to access this S3 bucket.

**Example**

```
  terraform:
    state_bucket_enabled: true
    state_bucket_name: "tfstate"
    state_bucket_key: "123456/terraform.tfstate"
    state_bucket_region: "us-east-1"
    state_bucket_endpoint: "https://nyc3.digitaloceanspaces.com"
    bucket_access_key: "{{lookup('community.general.lastpass', 'Business/Digitalocean', field='access_key' )}}"
    bucket_secret_key: "{{lookup('community.general.lastpass', 'Business/Digitalocean', field='secret_key' )}}"
    digitalocean_token: "{{lookup('community.general.lastpass', 'Business/Digitalocean', field='token' )}}"
```



```
  cloud_enabled: true
    cloud_organization: 'warhorse'
    cloud_workspace: 'test'
```
