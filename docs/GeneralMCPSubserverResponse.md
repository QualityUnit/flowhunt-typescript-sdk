# GeneralMCPSubserverResponse

General response schema for MCP subserver binding

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**server_id** | **string** | ID of the MCP subserver | [default to undefined]
**name** | **string** | Name of the MCP subserver | [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**status** | **string** | Status of the MCP subserver | [default to undefined]
**icon** | **string** |  | [optional] [default to undefined]
**version** | **string** | Version of the MCP subserver | [default to undefined]
**capabilities** | [**Array&lt;GeneralMCPSubserverCapabilitiesResponse&gt;**](GeneralMCPSubserverCapabilitiesResponse.md) | List of capabilities for the MCP subserver | [optional] [default to undefined]
**integration_slug** | [**IntegrationSlug**](IntegrationSlug.md) |  | [default to undefined]

## Example

```typescript
import { GeneralMCPSubserverResponse } from 'flowhunt';

const instance: GeneralMCPSubserverResponse = {
    server_id,
    name,
    description,
    status,
    icon,
    version,
    capabilities,
    integration_slug,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
