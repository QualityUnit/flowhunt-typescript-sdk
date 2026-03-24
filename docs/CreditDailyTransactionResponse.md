# CreditDailyTransactionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **string** | Transactions from date | [default to undefined]
**workspace_id** | **string** | Workspace ID | [default to undefined]
**transaction_type** | [**TransactionType**](TransactionType.md) | Transaction type | [default to undefined]
**amount** | **number** | Amount of credits | [default to undefined]
**cnt** | **number** | Number of transactions | [default to undefined]

## Example

```typescript
import { CreditDailyTransactionResponse } from 'flowhunt';

const instance: CreditDailyTransactionResponse = {
    created_at,
    workspace_id,
    transaction_type,
    amount,
    cnt,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
