
# Response Region Response

*This model accepts additional fields of type unknown.*

## Structure

`ResponseRegionResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `region` | `string` | Required | - |
| `fleetApiBaseUrl` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "region": "region0",
  "fleet_api_base_url": "fleet_api_base_url8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

