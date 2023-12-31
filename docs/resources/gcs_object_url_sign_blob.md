---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "avgcp_gcs_object_url_sign_blob Resource - terraform-provider-avgcp"
subcategory: ""
description: |-
  Example resource
---

# avgcp_gcs_object_url_sign_blob (Resource)

Example resource

## Example Usage

```terraform
terraform {
  required_providers {
    avgcp = {
      source  = "terraform.local/local/avgcp"
      version = "1.0.0"
    }
  }
}

resource "avgcp_gcs_object_url_sign_blob" "example" {
  google_access_id = "tf-avgcp@homelab-X.iam.gserviceaccount.com"
  bucket           = "terraform_provider_avgcp"
  path             = "test"
}

output "signed_url" {
  value = avgcp_gcs_object_url_sign_blob.example.signed_url
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `bucket` (String) Example configurable attribute
- `path` (String) Example configurable attribute

### Optional

- `google_access_id` (String) Example configurable attribute

### Read-Only

- `signed_url` (String) Example identifier
