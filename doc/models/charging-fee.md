
# Charging Fee

*This model accepts additional fields of type unknown.*

## Structure

`ChargingFee`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `sessionFeeId` | `number \| undefined` | Optional | - |
| `feeType` | `string \| undefined` | Optional | - |
| `currencyCode` | `string \| undefined` | Optional | - |
| `pricingType` | `string \| undefined` | Optional | - |
| `rateBase` | `number \| undefined` | Optional | - |
| `rateTier1` | `number \| undefined` | Optional | - |
| `rateTier2` | `number \| undefined` | Optional | - |
| `rateTier3` | `number \| null \| undefined` | Optional | - |
| `rateTier4` | `number \| null \| undefined` | Optional | - |
| `usageBase` | `number \| undefined` | Optional | - |
| `usageTier1` | `number \| undefined` | Optional | - |
| `usageTier2` | `number \| undefined` | Optional | - |
| `usageTier3` | `number \| null \| undefined` | Optional | - |
| `usageTier4` | `number \| null \| undefined` | Optional | - |
| `totalBase` | `number \| undefined` | Optional | - |
| `totalTier1` | `number \| undefined` | Optional | - |
| `totalTier2` | `number \| undefined` | Optional | - |
| `totalTier3` | `number \| undefined` | Optional | - |
| `totalTier4` | `number \| undefined` | Optional | - |
| `totalDue` | `number \| undefined` | Optional | - |
| `netDue` | `number \| undefined` | Optional | - |
| `uom` | `string \| undefined` | Optional | - |
| `isPaid` | `boolean \| undefined` | Optional | - |
| `status` | `string \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "sessionFeeId": 236,
  "feeType": "feeType4",
  "currencyCode": "currencyCode0",
  "pricingType": "pricingType6",
  "rateBase": 226.56,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

