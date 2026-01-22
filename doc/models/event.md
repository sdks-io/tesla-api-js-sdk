
# Event

*This model accepts additional fields of type unknown.*

## Structure

`Event`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `timestamp` | `string` | Required | - |
| `duration` | `number` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "timestamp": "2016-03-13T12:52:32.123Z",
  "duration": 40,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

