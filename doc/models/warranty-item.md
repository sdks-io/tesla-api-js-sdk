
# Warranty Item

*This model accepts additional fields of type unknown.*

## Structure

`WarrantyItem`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `warrantyType` | `string \| undefined` | Optional | - |
| `warrantyDisplayName` | `string \| undefined` | Optional | - |
| `expirationDate` | `string \| undefined` | Optional | - |
| `expirationOdometer` | `number \| undefined` | Optional | - |
| `odometerUnit` | `string \| undefined` | Optional | - |
| `warrantyExpiredOn` | `string \| null \| undefined` | Optional | - |
| `coverageAgeInYears` | `number \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "warrantyType": "warrantyType8",
  "warrantyDisplayName": "warrantyDisplayName0",
  "expirationDate": "2016-03-13T12:52:32.123Z",
  "expirationOdometer": 224,
  "odometerUnit": "odometerUnit6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

