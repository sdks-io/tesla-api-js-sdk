
# Adjust Volume Request

*This model accepts additional fields of type unknown.*

## Structure

`AdjustVolumeRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `volume` | `number` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "volume": 110,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

