
# Enterprise Payer Request

*This model accepts additional fields of type unknown.*

## Structure

`EnterprisePayerRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `role` | `string` | Required | - |
| `federationId` | `string \| undefined` | Optional | - |
| `accountId` | `string \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "role": "role0",
  "federation_id": "federation_id0",
  "account_id": "account_id8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

