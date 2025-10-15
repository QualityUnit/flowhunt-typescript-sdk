# UserResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **string** | User ID | [default to undefined]
**email** | **string** | Email of the user | [default to undefined]
**username** | **string** | Name of the user | [default to undefined]
**is_active** | **boolean** |  | [optional] [default to undefined]
**avatar_url** | **string** |  | [optional] [default to undefined]
**api_key_workspace_id** | **string** |  | [optional] [default to undefined]
**product_plans** | [**{ [key: string]: SubscriptionPlan; }**](SubscriptionPlan.md) |  | [optional] [default to undefined]
**billing_provider** | [**BillingProvider**](BillingProvider.md) |  | [optional] [default to undefined]

## Example

```typescript
import { UserResponse } from 'flowhunt';

const instance: UserResponse = {
    user_id,
    email,
    username,
    is_active,
    avatar_url,
    api_key_workspace_id,
    product_plans,
    billing_provider,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
