
# Api 1 Dx Vehicles Options Response

*This model accepts additional fields of type unknown.*

## Structure

`Api1DxVehiclesOptionsResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `response` | [`ResponseApi1DxVehiclesOptionsResponse \| undefined`](../../doc/models/response-api-1-dx-vehicles-options-response.md) | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "response": {
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

