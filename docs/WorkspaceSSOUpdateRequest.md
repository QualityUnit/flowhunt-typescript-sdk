# WorkspaceSSOUpdateRequest

Request DTO for updating workspace SSO settings.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **boolean** | Whether SSO is enabled | [optional] [default to true]
**idp_sso_url** | **string** |  | [optional] [default to undefined]
**idp_entity_id** | **string** |  | [optional] [default to undefined]
**idp_x509_cert** | **string** |  | [optional] [default to undefined]
**jit_provisioning_enabled** | **boolean** | Enable Just-In-Time user provisioning | [optional] [default to false]
**email_attribute** | **string** |  | [optional] [default to undefined]
**name_id_format** | **string** |  | [optional] [default to undefined]
**first_name_attribute** | **string** |  | [optional] [default to undefined]
**last_name_attribute** | **string** |  | [optional] [default to undefined]
**role_attribute** | **string** |  | [optional] [default to undefined]
**login_method** | [**SamlLoginMethod**](SamlLoginMethod.md) |  | [optional] [default to undefined]
**idp_metadata_xml** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { WorkspaceSSOUpdateRequest } from 'flowhunt';

const instance: WorkspaceSSOUpdateRequest = {
    enabled,
    idp_sso_url,
    idp_entity_id,
    idp_x509_cert,
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
