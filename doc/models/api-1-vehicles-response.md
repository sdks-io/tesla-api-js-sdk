
# Api 1 Vehicles Response

*This model accepts additional fields of type unknown.*

## Structure

`Api1VehiclesResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `response` | [`VehicleBase[] \| undefined`](../../doc/models/vehicle-base.md) | Optional | - |
| `pagination` | [`Pagination \| undefined`](../../doc/models/pagination.md) | Optional | - |
| `count` | `number \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "response": [
    {
      "id": 206,
      "vehicle_id": 56,
      "vin": "vin6",
      "display_name": "display_name0",
      "access_type": "access_type4",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "pagination": {
    "previous": 66,
    "next": 156,
    "current": 130,
    "per_page": 54,
    "count": 192,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "count": 14,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

