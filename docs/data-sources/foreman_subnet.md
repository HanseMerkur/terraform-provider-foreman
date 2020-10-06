
# foreman_subnet


Foreman representation of a subnetwork.


## Example Usage

```
# Autogenerated example with required keys
data "foreman_subnet" "example" {
  name = "public"
  network = "10.228.247.0"
}
```


## Argument Reference

The following arguments are supported:

- `name` - (Optional) Name of a subnetwork.
- `network` - (Optional) Subnet network.


## Attributes Reference

The following attributes are exported:

- `boot_mode` - Default boot mode for instances assigned to this subnet. Values include: `"Static"`, `"DHCP"`.
- `dns_primary` - Primary DNS server for this subnet.
- `dns_secondary` - Secondary DNS sever for this subnet.
- `from` - Start IP address for IP auto suggestion.
- `gateway` - Gateway server to use when connecting/communicating to anything not on the same network.
- `ipam` - IP address auto-suggestion for this subnet. Valid values include: `"DHCP"`, `"Internal DB"`, `"None"`.
- `mask` - Netmask for this subnet.
- `name` - Name of a subnetwork.
- `network` - Subnet network.
- `network_address` - The Subnets CIDR in the format 169.254.0.0/16
- `to` - Ending IP address for IP auto suggestion.
