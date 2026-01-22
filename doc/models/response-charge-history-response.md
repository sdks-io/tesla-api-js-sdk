
# Response Charge History Response

*This model accepts additional fields of type unknown.*

## Structure

`ResponseChargeHistoryResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `chargeHistory` | [`ChargeHistory[]`](../../doc/models/charge-history.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "charge_history": [
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
      "energy_added_wh": 56,
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

