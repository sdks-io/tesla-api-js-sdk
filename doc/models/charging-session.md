
# Charging Session

*This model accepts additional fields of type unknown.*

## Structure

`ChargingSession`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `string \| undefined` | Optional | - |
| `vin` | `string \| undefined` | Optional | - |
| `model` | `string \| undefined` | Optional | - |
| `startDateTime` | `string \| undefined` | Optional | - |
| `stopDateTime` | `string \| undefined` | Optional | - |
| `totalEnergy` | `number \| undefined` | Optional | - |
| `totalTime` | `number \| undefined` | Optional | - |
| `totalCost` | [`TotalCost \| undefined`](../../doc/models/total-cost.md) | Optional | - |
| `location` | [`Location \| undefined`](../../doc/models/location.md) | Optional | - |
| `chargingPeriods` | [`ChargingPeriod[] \| undefined`](../../doc/models/charging-period.md) | Optional | - |
| `tariffs` | [`Tariffs \| undefined`](../../doc/models/tariffs.md) | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "id": "id0",
  "vin": "vin6",
  "model": "model8",
  "start_date_time": "start_date_time6",
  "stop_date_time": "stop_date_time2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

