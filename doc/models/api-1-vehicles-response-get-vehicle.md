
# Api 1 Vehicles Response Get Vehicle

*This model accepts additional fields of type unknown.*

## Structure

`Api1VehiclesResponseGetVehicle`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `response` | [`VehicleBase \| undefined`](../../doc/models/vehicle-base.md) | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "response": {
    "id": 206,
    "vehicle_id": 56,
    "vin": "vin6",
    "display_name": "display_name0",
    "access_type": "access_type4",
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

