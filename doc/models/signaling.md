
# Signaling

*This model accepts additional fields of type unknown.*

## Structure

`Signaling`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `enabled` | `boolean` | Required | - |
| `subscribeConnectivity` | `boolean` | Required | - |
| `useAuthToken` | `boolean` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "enabled": false,
  "subscribe_connectivity": false,
  "use_auth_token": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

