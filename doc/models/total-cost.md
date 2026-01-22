
# Total Cost

*This model accepts additional fields of type unknown.*

## Structure

`TotalCost`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `exclVat` | `number \| undefined` | Optional | - |
| `inclVat` | `number \| undefined` | Optional | - |
| `vat` | `number \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "excl_vat": 13.82,
  "incl_vat": 65.46,
  "vat": 170.96,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

