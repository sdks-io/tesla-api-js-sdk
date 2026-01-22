
# Driver

*This model accepts additional fields of type unknown.*

## Structure

`Driver`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `myTeslaUniqueId` | `number \| undefined` | Optional | - |
| `userId` | `number \| undefined` | Optional | - |
| `userIdS` | `string \| undefined` | Optional | - |
| `vaultUuid` | `string \| undefined` | Optional | - |
| `driverFirstName` | `string \| undefined` | Optional | - |
| `driverLastName` | `string \| undefined` | Optional | - |
| `granularAccess` | `unknown \| undefined` | Optional | - |
| `activePubkeys` | `string[] \| undefined` | Optional | - |
| `publicKey` | `string \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "my_tesla_unique_id": 40,
  "user_id": 64,
  "user_id_s": "user_id_s4",
  "vault_uuid": "vault_uuid0",
  "driver_first_name": "driver_first_name2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

