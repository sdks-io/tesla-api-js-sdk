
# Response Fleet Telemetry Errors Response

*This model accepts additional fields of type unknown.*

## Structure

`ResponseFleetTelemetryErrorsResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `fleetTelemetryErrors` | [`FleetTelemetryError[]`](../../doc/models/fleet-telemetry-error.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "fleet_telemetry_errors": [
    {
      "name": "name8",
      "error": "error2",
      "vin": "vin8",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

