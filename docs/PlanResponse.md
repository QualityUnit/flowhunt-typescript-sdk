# PlanResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**plans** | **{ [key: string]: Array&lt;PlanListItemResponse&gt;; }** |  | [default to undefined]
**billing_provider** | [**BillingProvider**](BillingProvider.md) |  | [optional] [default to undefined]
**shopify_manage_url** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { PlanResponse } from 'flowhunt';

const instance: PlanResponse = {
    plans,
    billing_provider,
    shopify_manage_url,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
