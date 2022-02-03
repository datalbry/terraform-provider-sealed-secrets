---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "sealed_secret Data Source - terraform-provider-sealed-secrets"
subcategory: ""
description: |-
  Creates a sealed secret and stores it in yaml_content.
---

# sealed_secret (Data Source)

Creates a sealed secret and stores it in yaml_content.



<!-- schema generated by tfplugindocs -->
## Schema

### Required

- **name** (String) Name of the secret, must be unique.
- **namespace** (String) Namespace of the secret.

### Optional

- **data** (Map of String, Sensitive) Key/value pairs to populate the secret. The value will be base64 encoded
- **id** (String) The ID of this resource.
- **secret_type** (String) The secret type (ex. Opaque). Default type is Opaque.

### Read-Only

- **public_key_hash** (String) The public key hashed to detect if the public key changes.
- **yaml_content** (String) The produced sealed secret yaml file.

