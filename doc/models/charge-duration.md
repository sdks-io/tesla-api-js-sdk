
# Charge Duration

*This model accepts additional fields of type unknown.*

## Structure

`ChargeDuration`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `seconds` | `number` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "seconds": 60,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

