
# Vehicle Base

*This model accepts additional fields of type unknown.*

## Structure

`VehicleBase`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `number \| undefined` | Optional | - |
| `vehicleId` | `number \| undefined` | Optional | - |
| `vin` | `string \| undefined` | Optional | - |
| `displayName` | `string \| undefined` | Optional | - |
| `accessType` | `string \| undefined` | Optional | - |
| `state` | `string \| undefined` | Optional | - |
| `inService` | `boolean \| undefined` | Optional | - |
| `calendarEnabled` | `boolean \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "id": 126,
  "vehicle_id": 120,
  "vin": "vin8",
  "display_name": "display_name4",
  "access_type": "access_type0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

