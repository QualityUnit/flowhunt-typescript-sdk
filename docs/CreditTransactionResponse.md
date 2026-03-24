# CreditTransactionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**transaction_id** | **string** | Transaction ID | [default to undefined]
**workspace_id** | **string** | Workspace ID | [default to undefined]
**user_id** | **string** | User ID or user to whom is transaction assigned | [default to undefined]
**created_at** | **string** | Transaction creation date | [default to undefined]
**transaction_type** | [**TransactionType**](TransactionType.md) | Transaction type | [default to undefined]
**context_id** | **string** | Context ID - identification of transaction context - eg chatbot id | [default to undefined]
**context_desc** | **string** | Context description - description of transaction context | [optional] [default to undefined]
**amount** | **number** | Amount of credits | [default to undefined]

## Example

```typescript
import { CreditTransactionResponse } from 'flowhunt';

const instance: CreditTransactionResponse = {
    transaction_id,
    workspace_id,
    user_id,
    created_at,
    transaction_type,
    context_id,
    context_desc,
    amount,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
