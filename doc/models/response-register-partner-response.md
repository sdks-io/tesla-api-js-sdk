
# Response Register Partner Response

*This model accepts additional fields of type unknown.*

## Structure

`ResponseRegisterPartnerResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `clientId` | `string` | Required | - |
| `name` | `string` | Required | - |
| `description` | `string \| undefined` | Optional | - |
| `domain` | `string` | Required | - |
| `ca` | `string \| null \| undefined` | Optional | - |
| `createdAt` | `string` | Required | - |
| `updatedAt` | `string` | Required | - |
| `enterpriseTier` | `string` | Required | - |
| `accountId` | `string` | Required | - |
| `issuer` | `string \| null \| undefined` | Optional | - |
| `csr` | `string \| null \| undefined` | Optional | - |
| `csrUpdatedAt` | `string \| null \| undefined` | Optional | - |
| `publicKey` | `string` | Required | - |
| `publicKeyHash` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "client_id": "client_id6",
  "name": "name4",
  "description": "description4",
  "domain": "domain0",
  "ca": "ca8",
  "created_at": "2016-03-13T12:52:32.123Z",
  "updated_at": "2016-03-13T12:52:32.123Z",
  "enterprise_tier": "enterprise_tier8",
  "account_id": "account_id6",
  "issuer": "issuer4",
  "csr": "csr6",
  "csr_updated_at": "2016-03-13T12:52:32.123Z",
  "public_key": "public_key2",
  "public_key_hash": "public_key_hash2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

