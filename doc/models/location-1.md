
# Location 1

*This model accepts additional fields of type unknown.*

## Structure

`Location1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `lat` | `number \| undefined` | Optional | - |
| `mLong` | `number \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "lat": 224.48,
  "long": 54.54,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

