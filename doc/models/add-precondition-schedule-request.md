
# Add Precondition Schedule Request

*This model accepts additional fields of type unknown.*

## Structure

`AddPreconditionScheduleRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `lat` | `number` | Required | - |
| `lon` | `number` | Required | - |
| `id` | `number` | Required | - |
| `daysOfWeek` | `string \| undefined` | Optional | - |
| `preconditionTime` | `number \| undefined` | Optional | - |
| `oneTime` | `boolean \| undefined` | Optional | - |
| `enabled` | `boolean` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "lat": 87.82,
  "lon": 176.92,
  "id": 62,
  "days_of_week": "days_of_week8",
  "precondition_time": 70,
  "one_time": false,
  "enabled": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

