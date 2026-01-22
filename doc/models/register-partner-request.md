
# Register Partner Request

*This model accepts additional fields of type unknown.*

## Structure

`RegisterPartnerRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `domain` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "domain": "domain.com",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

