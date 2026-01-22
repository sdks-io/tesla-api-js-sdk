
# Fleet Telemetry Error

*This model accepts additional fields of type unknown.*

## Structure

`FleetTelemetryError`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `name` | `string` | Required | - |
| `error` | `string` | Required | - |
| `vin` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "name": "name2",
  "error": "error6",
  "vin": "vin6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

