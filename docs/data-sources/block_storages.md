---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "scp_block_storages Data Source - scp"
subcategory: ""
description: |-
  Provides list of block storages
---

# scp_block_storages (Data Source)

Provides list of block storages

## Example Usage

```terraform
data "scp_block_storages" "my_scp_block_storages" {
}

output "output_my_scp_block_storages" {
  value = data.scp_block_storages.my_scp_block_storages
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Optional

- `created_by` (String) The person who created the resource
- `page` (Number) Page start number from which to get the list
- `size` (Number) Size to get list
- `virtual_server_id` (String) Virtual server id

### Read-Only

- `contents` (Block List) Block Storage list (see [below for nested schema](#nestedblock--contents))
- `id` (String) The ID of this resource.
- `total_count` (Number) Total list size

<a id="nestedblock--contents"></a>
### Nested Schema for `contents`

Read-Only:

- `block_id` (String) Block id of this region
- `block_storage_id` (String) Block Storage id
- `block_storage_name` (String) Block storage name to create.
- `block_storage_size` (Number) Storage size(GB)
- `block_storage_state` (String) Block storage status
- `block_storage_uuid` (String) Block Storage uuid
- `created_by` (String) Person who created the resource
- `created_dt` (String) Creation time
- `device_node` (String) Device node
- `encrypt_enabled` (Boolean) Enable encryption feature in storage
- `is_boot_disk` (Boolean) Check whether it is OS(Boot) disk or not
- `modified_by` (String) Person who modified the resource
- `modified_dt` (String) Modification time
- `mount_path` (String) Mount path
- `product_id` (String) Product id of block storage
- `project_id` (String) Project id
- `service_zone_id` (String) Service zone id
- `shared_type` (String) Shared type of block storage
- `virtual_server_id` (String) Virtual server id to assign the block storage.

