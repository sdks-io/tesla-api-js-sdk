
# Guest Mode Request

*This model accepts additional fields of type unknown.*

## Structure

`GuestModeRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `enable` | `boolean` | Required | Enable or disable Guest Mode |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "enable": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

