
# Operation Request

*This model accepts additional fields of type unknown.*

## Structure

`OperationRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `defaultRealMode` | [`DefaultRealMode`](../../doc/models/default-real-mode.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "default_real_mode": "autonomous",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

