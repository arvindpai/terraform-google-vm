# umig-static-ips

This is an example to demonstrate how to use the UMIG module to create unmanaged
instance groups with user-specified static IPs.

[^]: (autogen_docs_start)

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| credentials\_path | The path to the GCP credentials JSON file | string | n/a | yes |
| num\_instances | Number of instances to create | string | `"1"` | no |
| project\_id | The GCP project to use for integration tests | string | n/a | yes |
| region | The GCP region to create and test resources in | string | n/a | yes |
| service\_account | Service account email address and scopes | map | n/a | yes |
| static\_ips | List of static IPs for VM instances | list | n/a | yes |
| subnetwork | The subnetwork to host the compute instances in | string | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| available\_zones | List of available zones in region |
| instances\_self\_links | List of self-links for compute instances |
| self\_links | List of self-links of unmanaged instance groups |

[^]: (autogen_docs_end)