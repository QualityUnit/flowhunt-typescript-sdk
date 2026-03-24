# CustomerDataRequestPayload


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**shop_id** | **number** |  | [default to undefined]
**shop_domain** | **string** |  | [default to undefined]
**orders_requested** | **Array&lt;number&gt;** |  | [default to undefined]
**customer** | **{ [key: string]: any; }** |  | [default to undefined]
**data_request** | **{ [key: string]: any; }** |  | [default to undefined]

## Example

```typescript
import { CustomerDataRequestPayload } from 'flowhunt';

const instance: CustomerDataRequestPayload = {
    shop_id,
    shop_domain,
    orders_requested,
    customer,
    data_request,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
