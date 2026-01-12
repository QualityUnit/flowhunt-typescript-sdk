# CreditTransactionSearchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**transaction_id** | **string** |  | [optional] [default to undefined]
**created_at_from** | **string** |  | [optional] [default to undefined]
**created_at_to** | **string** |  | [optional] [default to undefined]
**transaction_type** | [**TransactionType**](TransactionType.md) |  | [optional] [default to undefined]
**context_id** | **string** |  | [optional] [default to undefined]
**context_desc** | **string** |  | [optional] [default to undefined]
**limit** | **number** |  | [optional] [default to undefined]
**pagination** | [**Pagination**](Pagination.md) |  | [optional] [default to undefined]

## Example

```typescript
import { CreditTransactionSearchRequest } from 'flowhunt';

const instance: CreditTransactionSearchRequest = {
    transaction_id,
    created_at_from,
    created_at_to,
    transaction_type,
    context_id,
    context_desc,
    limit,
    pagination,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
