---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "scp_iam_role Data Source - scp"
subcategory: ""
description: |-
  
---

# scp_iam_role (Data Source)



## Example Usage

```terraform
data "scp_iam_role" "my_role" {
  role_id = "ROLE-XXXXX"
}

output "result_my_role" {
  value = data.scp_iam_role.my_role
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `role_id` (String) Role ID

### Read-Only

- `created_by` (String) Creator's ID
- `created_by_email` (String) Creator's email
- `created_by_name` (String) Creator's name
- `created_dt` (String) Created date
- `description` (String) Description
- `id` (String) The ID of this resource.
- `modified_by` (String) Modifier's ID
- `modified_by_email` (String) Modifier's email
- `modified_by_name` (String) Modifier's name
- `modified_dt` (String) Modified date
- `project_id` (String) Project ID
- `role_name` (String) Role name
- `role_policy_count` (Number) Description
- `role_srn` (String) Role SRN
- `session_time` (Number) Session time
- `tags` (List of Object) Tag list (see [below for nested schema](#nestedatt--tags))
- `trust_principals` (Set of Object) Performing subjects (see [below for nested schema](#nestedatt--trust_principals))

<a id="nestedatt--tags"></a>
### Nested Schema for `tags`

Read-Only:

- `tag_key` (String)
- `tag_value` (String)


<a id="nestedatt--trust_principals"></a>
### Nested Schema for `trust_principals`

Read-Only:

- `project_ids` (List of String)
- `user_srns` (List of String)

