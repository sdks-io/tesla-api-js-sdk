
# Charging Location

*This model accepts additional fields of type unknown.*

## Structure

`ChargingLocation`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `name` | `string \| undefined` | Optional | - |
| `type` | `string \| undefined` | Optional | - |
| `distanceMiles` | `number \| undefined` | Optional | - |
| `amenities` | `string \| undefined` | Optional | - |
| `availableStalls` | `number \| undefined` | Optional | - |
| `totalStalls` | `number \| undefined` | Optional | - |
| `siteClosed` | `boolean \| undefined` | Optional | - |
| `billingInfo` | `string \| undefined` | Optional | - |
| `location` | [`Location1 \| undefined`](../../doc/models/location-1.md) | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "name": "name0",
  "type": "type0",
  "distance_miles": 123.84,
  "amenities": "amenities0",
  "available_stalls": 60,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

