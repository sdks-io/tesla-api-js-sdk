
# Backup Request

*This model accepts additional fields of type unknown.*

## Structure

`BackupRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `backupReservePercent` | `number` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "backup_reserve_percent": 32,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

