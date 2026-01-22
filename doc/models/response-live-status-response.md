
# Response Live Status Response

*This model accepts additional fields of type unknown.*

## Structure

`ResponseLiveStatusResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `solarPower` | `number` | Required | - |
| `energyLeft` | `number` | Required | - |
| `totalPackEnergy` | `number` | Required | - |
| `percentageCharged` | `number` | Required | - |
| `backupCapable` | `boolean` | Required | - |
| `batteryPower` | `number \| undefined` | Optional | - |
| `loadPower` | `number \| undefined` | Optional | - |
| `gridStatus` | `string \| undefined` | Optional | - |
| `gridPower` | `number \| undefined` | Optional | - |
| `islandStatus` | `string \| undefined` | Optional | - |
| `stormModeActive` | `boolean \| undefined` | Optional | - |
| `timestamp` | `string \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "solar_power": 108.14,
  "energy_left": 185.46,
  "total_pack_energy": 65.2,
  "percentage_charged": 141.22,
  "backup_capable": false,
  "battery_power": 211.48,
  "load_power": 248.74,
  "grid_status": "grid_status2",
  "grid_power": 38.0,
  "island_status": "island_status4",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

