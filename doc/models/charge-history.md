
# Charge History

*This model accepts additional fields of type unknown.*

## Structure

`ChargeHistory`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `chargeStartTime` | [`ChargeStartTime`](../../doc/models/charge-start-time.md) | Required | - |
| `chargeDuration` | [`ChargeDuration`](../../doc/models/charge-duration.md) | Required | - |
| `energyAddedWh` | `number` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "charge_start_time": {
    "seconds": 206,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "charge_duration": {
    "seconds": 62,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "energy_added_wh": 176,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

