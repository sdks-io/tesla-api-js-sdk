
# Actuate Trunk Request

*This model accepts additional fields of type unknown.*

## Structure

`ActuateTrunkRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `whichTrunk` | [`WhichTrunk`](../../doc/models/which-trunk.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "which_trunk": "front",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

