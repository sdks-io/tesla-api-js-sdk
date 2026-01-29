
# Command Result

*This model accepts additional fields of type unknown.*

## Structure

`CommandResult`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `result` | `boolean` | Required | - |
| `reason` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "result": false,
  "reason": "reason0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

