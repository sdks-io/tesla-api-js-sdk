
# Public Key Response

*This model accepts additional fields of type unknown.*

## Structure

`PublicKeyResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `response` | [`ResponsePublicKeyResponse`](../../doc/models/response-public-key-response.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "response": {
    "public_key": "public_key6",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

