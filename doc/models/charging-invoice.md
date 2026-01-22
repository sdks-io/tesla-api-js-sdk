
# Charging Invoice

*This model accepts additional fields of type unknown.*

## Structure

`ChargingInvoice`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `fileName` | `string \| undefined` | Optional | - |
| `contentId` | `string \| undefined` | Optional | - |
| `invoiceType` | `string \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "fileName": "fileName0",
  "contentId": "contentId0",
  "invoiceType": "invoiceType0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

