# Data

Document linked to vector

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**schedule_id** | **string** |  | [default to undefined]
**domain_id** | **string** |  | [default to undefined]
**url_id** | **string** |  | [default to undefined]
**url** | **string** |  | [default to undefined]
**last_text_timestamp** | **string** |  | [default to undefined]
**page_screenshot** | [**UrlScreenshotResponse**](UrlScreenshotResponse.md) |  | [default to undefined]
**url_title** | **string** |  | [default to undefined]
**url_meta_description** | **string** |  | [default to undefined]
**url_og_image** | **string** |  | [default to undefined]
**is_original_url** | **boolean** |  | [default to undefined]
**dest_url_id** | **string** |  | [default to undefined]
**created_at** | **string** |  | [default to undefined]
**url_text** | **Array&lt;{ [key: string]: string; }&gt;** |  | [default to undefined]
**faq_id** | **string** | FAQ ID | [default to undefined]
**workspace_id** | **string** | Workspace ID | [default to undefined]
**cat_id** | **string** | Category ID | [default to undefined]
**question** | **string** | Question | [default to undefined]
**answer** | **string** |  | [optional] [default to undefined]
**parent_faq_id** | **string** |  | [optional] [default to undefined]
**status** | **string** | Document status | [default to undefined]
**updated_at** | **string** | Document updated at | [default to undefined]
**indexed_at** | **string** |  | [optional] [default to undefined]
**doc_id** | **string** | Document ID | [default to undefined]
**doc_name** | **string** | Document name | [default to undefined]
**doc_type** | **string** | Document type | [default to undefined]
**user_status** | **string** | User status | [default to undefined]

## Example

```typescript
import { Data } from 'flowhunt';

const instance: Data = {
    schedule_id,
    domain_id,
    url_id,
    url,
    last_text_timestamp,
    page_screenshot,
    url_title,
    url_meta_description,
    url_og_image,
    is_original_url,
    dest_url_id,
    created_at,
    url_text,
    faq_id,
    workspace_id,
    cat_id,
    question,
    answer,
    parent_faq_id,
    status,
    updated_at,
    indexed_at,
    doc_id,
    doc_name,
    doc_type,
    user_status,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
