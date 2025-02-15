+++
title = "ChefWindowsPlatformHelper"

+++

<!-- This content is automatically generated. See https://github.com/chef/chef-web-docs/blob/main/generated/README.md -->

The department is: `ChefWindowsPlatformHelper`

The full name of the cop is: `Chef/Deprecations/ChefWindowsPlatformHelper`

| Enabled by default | Supports autocorrection | Target Chef Version |
| --- | --- | --- |
| Enabled | Yes | All Versions |

Use `platform?('windows')` instead of the legacy `Chef::Platform.windows?` helper

## Examples


#### incorrect

```ruby
Chef::Platform.windows?
```

#### correct

```ruby
platform?('windows')
platform_family?('windows')
```

## Configurable attributes

<table>
<tbody><tr>
<th>Name</th>
<th>Default value</th>
<th>Configurable values</th>
</tr>
<tr>
<td style="text-align:center">Version Added</td>
<td style="text-align:center">6.0.0</td>
<td style="text-align:center">String</td>
</tr>
<tr><td style="text-align:center">Include</td>
<td style="text-align:center"><ul>
</ul>
</td>
<td style="text-align:center">Array</td>
</tr></tbody></table>
