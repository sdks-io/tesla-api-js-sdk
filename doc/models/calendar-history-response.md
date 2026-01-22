
# Calendar History Response

*This model accepts additional fields of type unknown.*

## Structure

`CalendarHistoryResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `response` | [`ResponseCalendarHistoryResponse`](../../doc/models/response-calendar-history-response.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "response": {
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
    "total_events": 236,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

