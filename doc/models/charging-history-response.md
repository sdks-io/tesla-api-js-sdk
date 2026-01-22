
# Charging History Response

*This model accepts additional fields of type unknown.*

## Structure

`ChargingHistoryResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `response` | [`ChargingHistoryData`](../../doc/models/charging-history-data.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "response": {
    "data": [
      {
        "sessionId": 186,
        "vin": "vin4",
        "siteLocationName": "siteLocationName6",
        "chargeStartDateTime": "2016-03-13T12:52:32.123Z",
        "chargeStopDateTime": "2016-03-13T12:52:32.123Z",
        "unlatchDateTime": "2016-03-13T12:52:32.123Z",
        "countryCode": "countryCode6",
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
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

