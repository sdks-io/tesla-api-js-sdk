
# Pagination

*This model accepts additional fields of type unknown.*

## Structure

`Pagination`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `previous` | `number \| null \| undefined` | Optional | - |
| `next` | `number \| null \| undefined` | Optional | - |
| `current` | `number \| undefined` | Optional | - |
| `perPage` | `number \| undefined` | Optional | - |
| `count` | `number \| undefined` | Optional | - |
| `pages` | `number \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "previous": 176,
  "next": 10,
  "current": 16,
  "per_page": 92,
  "count": 210,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

