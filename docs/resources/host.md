---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "bindrole_host Resource - terraform-provider-bindrole"
subcategory: ""
description: |-
  Represents a host entry in a domain as a hostvar
---

# bindrole_host (Resource)

Represents a host entry in a domain as a hostvar

## Example Usage

```terraform
resource "bindrole_host" "netsrv-01" {
  domain   = "my.domain.tld"
  hostname = "netsrv-01"
  ip       = "10.0.0.1"
  aliases = [
    "ns-01",
    "dhcp-01"
  ]
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `domain` (String) The fqn of the domain this host is in
- `hostname` (String) The hostname (only) for this host
- `ip` (String) The IP Address for this host

### Optional

- `aliases` (List of String) A list of aliases for this host

### Read-Only

- `id` (String) The ID of this resource.


