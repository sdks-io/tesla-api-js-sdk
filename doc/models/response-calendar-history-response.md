
# Response Calendar History Response

*This model accepts additional fields of type unknown.*

## Structure

`ResponseCalendarHistoryResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `events` | [`Event[]`](../../doc/models/event.md) | Required | - |
| `totalEvents` | `number` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "events": [
    {
      "timestamp": "2016-03-13T12:52:32.123Z",
      "duration": 68,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "total_events": 12,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

