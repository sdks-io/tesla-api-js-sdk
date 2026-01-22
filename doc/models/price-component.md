
# Price Component

*This model accepts additional fields of type unknown.*

## Structure

`PriceComponent`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `type` | `string \| undefined` | Optional | - |
| `price` | `number \| undefined` | Optional | - |
| `stepSize` | `number \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "type": "type2",
  "price": 87.54,
  "step_size": 214.68,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

