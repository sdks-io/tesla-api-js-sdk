
# Add Charge Schedule Request

*This model accepts additional fields of type unknown.*

## Structure

`AddChargeScheduleRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `lat` | `number` | Required | - |
| `lon` | `number` | Required | - |
| `id` | `number` | Required | - |
| `daysOfWeek` | `string \| undefined` | Optional | - |
| `startEnabled` | `boolean \| undefined` | Optional | - |
| `startTime` | `number \| undefined` | Optional | - |
| `endEnabled` | `boolean \| undefined` | Optional | - |
| `endTime` | `number \| undefined` | Optional | - |
| `oneTime` | `boolean \| undefined` | Optional | - |
| `enabled` | `boolean` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "lat": 196.62,
  "lon": 29.72,
  "id": 190,
  "days_of_week": "days_of_week8",
  "start_enabled": false,
  "start_time": 214,
  "end_enabled": false,
  "end_time": 174,
  "enabled": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

