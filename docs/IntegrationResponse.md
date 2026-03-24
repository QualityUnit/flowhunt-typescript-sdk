# IntegrationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**slug** | **string** | The slug of the integration. | [default to undefined]
**name** | **string** | The name of the integration. | [default to undefined]
**description** | **string** | The description of the integration. | [default to undefined]
**integrated_instance_cnt** | **number** | The number of integrated instances. | [default to undefined]
**categories** | [**Array&lt;IntegrationCategory&gt;**](IntegrationCategory.md) | The categories of the integration. | [default to undefined]
**alpha** | **boolean** | Whether the integration is in alpha or not. | [optional] [default to false]
**beta** | **boolean** | Whether the integration is in beta or not. | [optional] [default to false]
**public_flow_id** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { IntegrationResponse } from 'flowhunt';

const instance: IntegrationResponse = {
    slug,
    name,
    description,
    integrated_instance_cnt,
    categories,
    alpha,
    beta,
    public_flow_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
