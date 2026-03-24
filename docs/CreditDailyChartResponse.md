# CreditDailyChartResponse

Response containing chart data for daily credit transactions.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**per_day** | [**Array&lt;CreditDailyChartDataRow&gt;**](CreditDailyChartDataRow.md) | List of daily transaction data rows | [default to undefined]
**transaction_types** | [**Array&lt;TransactionType&gt;**](TransactionType.md) | List of all transaction type codes present in the data | [default to undefined]

## Example

```typescript
import { CreditDailyChartResponse } from 'flowhunt';

const instance: CreditDailyChartResponse = {
    per_day,
    transaction_types,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
