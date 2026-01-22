
# Charging History Item

*This model accepts additional fields of type unknown.*

## Structure

`ChargingHistoryItem`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `sessionId` | `number` | Required | - |
| `vin` | `string` | Required | - |
| `siteLocationName` | `string \| undefined` | Optional | - |
| `chargeStartDateTime` | `string \| undefined` | Optional | - |
| `chargeStopDateTime` | `string \| undefined` | Optional | - |
| `unlatchDateTime` | `string \| undefined` | Optional | - |
| `countryCode` | `string \| undefined` | Optional | - |
| `fees` | [`ChargingFee[] \| undefined`](../../doc/models/charging-fee.md) | Optional | - |
| `billingType` | `string \| undefined` | Optional | - |
| `invoices` | [`ChargingInvoice[] \| undefined`](../../doc/models/charging-invoice.md) | Optional | - |
| `vehicleMakeType` | `string \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "sessionId": 16,
  "vin": "vin0",
  "siteLocationName": "siteLocationName8",
  "chargeStartDateTime": "2016-03-13T12:52:32.123Z",
  "chargeStopDateTime": "2016-03-13T12:52:32.123Z",
  "unlatchDateTime": "2016-03-13T12:52:32.123Z",
  "countryCode": "countryCode8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

