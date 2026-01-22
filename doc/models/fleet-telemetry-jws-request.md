
# Fleet Telemetry Jws Request

*This model accepts additional fields of type unknown.*

## Structure

`FleetTelemetryJwsRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `token` | `string \| undefined` | Optional | - |
| `vins` | `string[] \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "token": "token8",
  "vins": [
    "vins0",
    "vins9",
    "vins8"
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

