+++
title = "MacosUserdefaultsGlobalProperty"

+++

<!-- This content is automatically generated. See https://github.com/chef/chef-web-docs/blob/main/generated/README.md -->

The department is: `MacosUserdefaultsGlobalProperty`

The full name of the cop is: `Chef/Deprecations/MacosUserdefaultsGlobalProperty`

| Enabled by default | Supports autocorrection | Target Chef Version |
| --- | --- | --- |
| Enabled | Yes | 16.3+ |

The `global` property in the macos_userdefaults resource was deprecated in Chef Infra Client 16.3. This property was never properly implemented and caused failures under many conditions. Omitting the `domain` property will now set global defaults.

## Examples


#### incorrect

```ruby
macos_userdefaults 'set a value' do
  global true
  key 'key'
  value 'value'
end
```

#### correct

```ruby
macos_userdefaults 'set a value' do
  key 'key'
  value 'value'
end
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
<td style="text-align:center">6.14.0</td>
<td style="text-align:center">String</td>
</tr>
<tr><td style="text-align:center">Include</td>
<td style="text-align:center"><ul>
</ul>
</td>
<td style="text-align:center">Array</td>
</tr></tbody></table>
