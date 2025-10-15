# FlowSessionCreateFromFlowRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **string** |  | [optional] [default to undefined]
**lang** | **string** |  | [optional] [default to undefined]
**access_token** | **string** |  | [optional] [default to undefined]
**refresh_token** | **string** |  | [optional] [default to undefined]
**username** | **string** |  | [optional] [default to undefined]
**password** | **string** |  | [optional] [default to undefined]
**variables** | **{ [key: string]: string; }** |  | [optional] [default to undefined]
**flow_id** | **string** | The flow ID | [default to undefined]
**on_chat_opened_postback_url** | **string** |  | [optional] [default to undefined]
**flow_branch** | [**FlowBranch**](FlowBranch.md) | The flow branch | [optional] [default to undefined]

## Example

```typescript
import { FlowSessionCreateFromFlowRequest } from 'flowhunt';

const instance: FlowSessionCreateFromFlowRequest = {
    url,
    lang,
    access_token,
    refresh_token,
    username,
    password,
    variables,
    flow_id,
    on_chat_opened_postback_url,
    flow_branch,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
