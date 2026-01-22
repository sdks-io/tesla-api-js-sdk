
# Response Orders Response

*This model accepts additional fields of type unknown.*

## Structure

`ResponseOrdersResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleMapId` | `number` | Required | - |
| `referenceNumber` | `string` | Required | - |
| `vin` | `string` | Required | - |
| `orderStatus` | `string` | Required | - |
| `orderSubstatus` | `string` | Required | - |
| `modelCode` | `string` | Required | - |
| `countryCode` | `string` | Required | - |
| `locale` | `string` | Required | - |
| `mktOptions` | `string` | Required | - |
| `isB2B` | `boolean` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "vehicleMapId": 198,
  "referenceNumber": "referenceNumber2",
  "vin": "vin8",
  "orderStatus": "orderStatus6",
  "orderSubstatus": "orderSubstatus2",
  "modelCode": "modelCode6",
  "countryCode": "countryCode6",
  "locale": "locale6",
  "mktOptions": "mktOptions2",
  "isB2b": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

