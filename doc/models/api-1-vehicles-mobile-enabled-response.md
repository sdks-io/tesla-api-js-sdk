
# Api 1 Vehicles Mobile Enabled Response

*This model accepts additional fields of type unknown.*

## Structure

`Api1VehiclesMobileEnabledResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `response` | [`MobileEnabled \| undefined`](../../doc/models/mobile-enabled.md) | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "response": {
    "result": false,
    "reason": "reason4",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

