# WorkspaceSSOCreateRequest

Request DTO for creating workspace SSO settings.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**provider** | **string** | SSO provider (e.g., \&#39;microsoft\&#39;) | [default to undefined]
**enabled** | **boolean** | Whether SSO is enabled | [optional] [default to true]
**idp_sso_url** | **string** | Identity Provider SSO URL | [optional] [default to undefined]
**jit_provisioning_enabled** | **boolean** |  | [optional] [default to undefined]
**email_attribute** | **string** |  | [optional] [default to undefined]
**name_id_format** | **string** |  | [optional] [default to undefined]
**first_name_attribute** | **string** |  | [optional] [default to undefined]
**last_name_attribute** | **string** |  | [optional] [default to undefined]
**role_attribute** | **string** |  | [optional] [default to undefined]
**login_method** | [**SamlLoginMethod**](SamlLoginMethod.md) |  | [optional] [default to undefined]
**idp_metadata_xml** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { WorkspaceSSOCreateRequest } from 'flowhunt';

const instance: WorkspaceSSOCreateRequest = {
    provider,
    enabled,
    idp_sso_url,
    jit_provisioning_enabled,
    email_attribute,
    name_id_format,
    first_name_attribute,
    last_name_attribute,
    role_attribute,
    login_method,
    idp_metadata_xml,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
