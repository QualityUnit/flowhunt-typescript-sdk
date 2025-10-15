# UserPlanResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**price_amount** | **number** |  | [default to undefined]
**price_currency** | **string** |  | [default to undefined]
**monthly_topup_credits** | **number** |  | [default to undefined]
**current_period_end** | **string** |  | [default to undefined]
**subscription_plans** | [**{ [key: string]: SubscriptionPlan; }**](SubscriptionPlan.md) |  | [default to undefined]
**can_remove_branding** | **boolean** |  | [default to undefined]
**extra_workspaces_count** | **number** |  | [optional] [default to undefined]
**extra_credits_count** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { UserPlanResponse } from 'flowhunt';

const instance: UserPlanResponse = {
    price_amount,
    price_currency,
    monthly_topup_credits,
    current_period_end,
    subscription_plans,
    can_remove_branding,
    extra_workspaces_count,
    extra_credits_count,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
