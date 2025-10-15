# PlanListItemResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**product_id** | **string** |  | [default to undefined]
**price_id** | **string** |  | [default to undefined]
**currency** | **string** |  | [default to undefined]
**amount_monthly** | **number** |  | [default to undefined]
**amount_yearly** | **number** |  | [optional] [default to undefined]
**recurring** | **boolean** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**description** | **string** |  | [default to undefined]
**popular** | **boolean** |  | [default to undefined]
**monthly_credits** | **number** |  | [default to undefined]
**features** | [**Array&lt;FeatureResponse&gt;**](FeatureResponse.md) |  | [default to undefined]
**subscription_plan** | [**SubscriptionPlan**](SubscriptionPlan.md) |  | [default to undefined]
**self_hosted** | **boolean** |  | [optional] [default to undefined]
**addon** | **boolean** |  | [optional] [default to undefined]
**addon_type** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { PlanListItemResponse } from 'flowhunt';

const instance: PlanListItemResponse = {
    product_id,
    price_id,
    currency,
    amount_monthly,
    amount_yearly,
    recurring,
    name,
    description,
    popular,
    monthly_credits,
    features,
    subscription_plan,
    self_hosted,
    addon,
    addon_type,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
