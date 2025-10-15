# WorkspaceSSOResponse

Response DTO for workspace SSO settings.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**workspace_id** | **string** |  | [default to undefined]
**provider** | **string** |  | [default to undefined]
**domain** | **string** |  | [default to undefined]
**enabled** | **boolean** |  | [default to undefined]
**created_at** | **string** |  | [default to undefined]
**updated_at** | **string** |  | [default to undefined]
**idp_sso_url** | **string** |  | [optional] [default to undefined]
**idp_metadata_xml** | **string** |  | [optional] [default to undefined]
**idp_entity_id** | **string** |  | [optional] [default to undefined]
**idp_x509_cert** | **string** |  | [optional] [default to undefined]
**login_method** | **string** |  | [optional] [default to undefined]
**jit_provisioning_enabled** | **boolean** |  | [optional] [default to false]
**email_attribute** | **string** |  | [optional] [default to undefined]
**name_id_format** | **string** |  | [optional] [default to undefined]
**assertion_consumer_service_url** | **string** |  | [optional] [default to undefined]
**first_name_attribute** | **string** |  | [optional] [default to undefined]
**last_name_attribute** | **string** |  | [optional] [default to undefined]
**role_attribute** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { WorkspaceSSOResponse } from 'flowhunt';

const instance: WorkspaceSSOResponse = {
    workspace_id,
    provider,
    domain,
    enabled,
    created_at,
    updated_at,
    idp_sso_url,
    idp_metadata_xml,
    idp_entity_id,
    idp_x509_cert,
    login_method,
    jit_provisioning_enabled,
    email_attribute,
    name_id_format,
    assertion_consumer_service_url,
    first_name_attribute,
    last_name_attribute,
    role_attribute,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
