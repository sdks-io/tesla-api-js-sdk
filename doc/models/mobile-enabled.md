
# Mobile Enabled

*This model accepts additional fields of type unknown.*

## Structure

`MobileEnabled`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `result` | `boolean \| undefined` | Optional | - |
| `reason` | `string \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "result": false,
  "reason": "reason2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

