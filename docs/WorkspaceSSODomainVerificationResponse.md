# WorkspaceSSODomainVerificationResponse

Response model for domain verification records.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**workspace_id** | **string** |  | [default to undefined]
**domain** | **string** |  | [default to undefined]
**nonce** | **string** |  | [default to undefined]
**verified** | **boolean** |  | [default to undefined]
**verification_hash** | **string** |  | [default to undefined]
**created_at** | **string** |  | [default to undefined]
**last_verified_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { WorkspaceSSODomainVerificationResponse } from 'flowhunt';

const instance: WorkspaceSSODomainVerificationResponse = {
    workspace_id,
    domain,
    nonce,
    verified,
    verification_hash,
    created_at,
    last_verified_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
