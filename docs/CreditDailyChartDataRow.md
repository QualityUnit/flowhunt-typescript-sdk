# CreditDailyChartDataRow

A single row in the chart data representing one day\'s transactions.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**date** | **string** | Date in YYYY-MM-DD format | [default to undefined]
**transaction_types** | **{ [key: string]: number; }** | Dictionary of transaction type codes to their total amounts | [default to undefined]

## Example

```typescript
import { CreditDailyChartDataRow } from 'flowhunt';

const instance: CreditDailyChartDataRow = {
    date,
    transaction_types,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
