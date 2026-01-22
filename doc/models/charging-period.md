
# Charging Period

*This model accepts additional fields of type unknown.*

## Structure

`ChargingPeriod`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `startDateTime` | `string \| undefined` | Optional | - |
| `dimensions` | [`ChargingDimension[] \| undefined`](../../doc/models/charging-dimension.md) | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "start_date_time": "start_date_time8",
  "dimensions": [
    {
      "type": "type6",
      "volume": 148.9,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "type": "type6",
      "volume": 148.9,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

