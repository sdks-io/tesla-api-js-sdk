
# Vehicle Option

*This model accepts additional fields of type unknown.*

## Structure

`VehicleOption`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `code` | `string \| undefined` | Optional | - |
| `displayName` | `string \| undefined` | Optional | - |
| `colorCode` | `string \| null \| undefined` | Optional | - |
| `isActive` | `boolean \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "code": "code2",
  "displayName": "displayName8",
  "colorCode": "colorCode4",
  "isActive": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

