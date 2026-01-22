
# Response Api 1 Dx Vehicles Options Response

*This model accepts additional fields of type unknown.*

## Structure

`ResponseApi1DxVehiclesOptionsResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `codes` | [`VehicleOption[] \| undefined`](../../doc/models/vehicle-option.md) | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "codes": [
    {
      "code": "code0",
      "displayName": "displayName0",
      "colorCode": "colorCode2",
      "isActive": false,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "code": "code0",
      "displayName": "displayName0",
      "colorCode": "colorCode2",
      "isActive": false,
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

