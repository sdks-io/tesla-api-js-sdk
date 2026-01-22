
# Response

*This model accepts additional fields of type unknown.*

## Structure

`Response`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `code` | `number` | Required | - |
| `message` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "code": 46,
  "message": "message4",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

