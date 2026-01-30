# V3ToolParameterResponse

Response schema for a tool parameter.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Parameter name | [default to undefined]
**display_name** | **string** | Display name for UI | [default to undefined]
**description** | **string** | Parameter description | [optional] [default to '']
**field_type** | **string** | V3 field type (e.g., \&#39;str\&#39;, \&#39;int\&#39;, \&#39;dict\&#39;) | [default to undefined]
**required** | **boolean** | Whether the parameter is required | [optional] [default to false]
**_default** | [****](.md) | Default value | [optional] [default to undefined]
**_options** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**range_spec** | **{ [key: string]: any; }** |  | [optional] [default to undefined]
**multiline** | **boolean** |  | [optional] [default to undefined]
**advanced** | **boolean** |  | [optional] [default to undefined]
**user_specified_param** | **boolean** | If True, parameter must be set by user, not AI agent | [optional] [default to false]
**loading_options_api** | **string** |  | [optional] [default to undefined]
**exclusive_group** | **string** |  | [optional] [default to undefined]
**exclusive_label** | **string** |  | [optional] [default to undefined]
**exclusive_order** | **number** |  | [optional] [default to undefined]
**exclusive_default** | **boolean** |  | [optional] [default to undefined]

## Example

```typescript
import { V3ToolParameterResponse } from 'flowhunt';

const instance: V3ToolParameterResponse = {
    name,
    display_name,
    description,
    field_type,
    required,
    _default,
    _options,
    range_spec,
    multiline,
    advanced,
    user_specified_param,
    loading_options_api,
    exclusive_group,
    exclusive_label,
    exclusive_order,
    exclusive_default,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
