# DocumentsApi

All URIs are relative to *https://api.flowhunt.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createDocumentCategory**](#createdocumentcategory) | **POST** /v2/documents/categories/create | Create Document Category|
|[**createFaq**](#createfaq) | **POST** /v2/documents/faqs/create | Create Faq|
|[**deleteDocument**](#deletedocument) | **DELETE** /v2/documents/{doc_id} | Delete Document|
|[**deleteDocumentCategory**](#deletedocumentcategory) | **DELETE** /v2/documents/categories/{cat_id} | Delete Document Category|
|[**deleteFaq**](#deletefaq) | **DELETE** /v2/documents/faqs/{faq_id} | Delete Faq|
|[**downloadBinaryDocument**](#downloadbinarydocument) | **GET** /v2/documents/download/binary/{doc_id} | Download Binary Document|
|[**downloadTextDocument**](#downloadtextdocument) | **GET** /v2/documents/download/text/{doc_id} | Download Text Document|
|[**importFaq**](#importfaq) | **POST** /v2/documents/faqs/import | Import Faq|
|[**searchDocumentCategories**](#searchdocumentcategories) | **POST** /v2/documents/categories/search | Search Document Categories|
|[**searchDocuments**](#searchdocuments) | **POST** /v2/documents/search | Search Documents|
|[**searchFaqs**](#searchfaqs) | **POST** /v2/documents/faqs/search | Search Faqs|
|[**updateDocument**](#updatedocument) | **PUT** /v2/documents/{doc_id} | Update Document|
|[**updateDocumentCategory**](#updatedocumentcategory) | **PUT** /v2/documents/categories/{cat_id} | Update Document Category|
|[**updateFaq**](#updatefaq) | **PUT** /v2/documents/faqs/{faq_id} | Update Faq|
|[**uploadFromUrlDocument**](#uploadfromurldocument) | **POST** /v2/documents/upload-from-url/{cat_id} | Upload From Url Document|
|[**uploadMemoryDocument**](#uploadmemorydocument) | **POST** /v2/documents/upload/{cat_id} | Upload Memory Document|

# **createDocumentCategory**
> DocumentCategoryResponse createDocumentCategory(documentCategoryCreateRequest)


### Example

```typescript
import {
    DocumentsApi,
    Configuration,
    DocumentCategoryCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new DocumentsApi(configuration);

let workspaceId: string; // (default to undefined)
let documentCategoryCreateRequest: DocumentCategoryCreateRequest; //

const { status, data } = await apiInstance.createDocumentCategory(
    workspaceId,
    documentCategoryCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **documentCategoryCreateRequest** | **DocumentCategoryCreateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**DocumentCategoryResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createFaq**
> Array<FaqResponse> createFaq(faqCreateRequest)


### Example

```typescript
import {
    DocumentsApi,
    Configuration,
    FaqCreateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new DocumentsApi(configuration);

let workspaceId: string; // (default to undefined)
let faqCreateRequest: FaqCreateRequest; //

const { status, data } = await apiInstance.createFaq(
    workspaceId,
    faqCreateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **faqCreateRequest** | **FaqCreateRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<FaqResponse>**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteDocument**
> Completed deleteDocument()


### Example

```typescript
import {
    DocumentsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new DocumentsApi(configuration);

let docId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteDocument(
    docId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **docId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Completed**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteDocumentCategory**
> Completed deleteDocumentCategory()


### Example

```typescript
import {
    DocumentsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new DocumentsApi(configuration);

let catId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteDocumentCategory(
    catId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **catId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Completed**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteFaq**
> Completed deleteFaq()


### Example

```typescript
import {
    DocumentsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new DocumentsApi(configuration);

let faqId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteFaq(
    faqId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **faqId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Completed**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **downloadBinaryDocument**
> any downloadBinaryDocument()


### Example

```typescript
import {
    DocumentsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new DocumentsApi(configuration);

let docId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.downloadBinaryDocument(
    docId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **docId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**any**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **downloadTextDocument**
> DocumentContent downloadTextDocument()


### Example

```typescript
import {
    DocumentsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new DocumentsApi(configuration);

let docId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)

const { status, data } = await apiInstance.downloadTextDocument(
    docId,
    workspaceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **docId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**DocumentContent**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **importFaq**
> FaqImportResponse importFaq()


### Example

```typescript
import {
    DocumentsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new DocumentsApi(configuration);

let workspaceId: string; // (default to undefined)
let file: File; // (default to undefined)

const { status, data } = await apiInstance.importFaq(
    workspaceId,
    file
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **file** | [**File**] |  | defaults to undefined|


### Return type

**FaqImportResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **searchDocumentCategories**
> Array<DocumentCategoryResponse> searchDocumentCategories(documentCategorySearchRequest)


### Example

```typescript
import {
    DocumentsApi,
    Configuration,
    DocumentCategorySearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new DocumentsApi(configuration);

let workspaceId: string; // (default to undefined)
let documentCategorySearchRequest: DocumentCategorySearchRequest; //

const { status, data } = await apiInstance.searchDocumentCategories(
    workspaceId,
    documentCategorySearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **documentCategorySearchRequest** | **DocumentCategorySearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<DocumentCategoryResponse>**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **searchDocuments**
> Array<DocumentResponse> searchDocuments(documentSearchRequest)


### Example

```typescript
import {
    DocumentsApi,
    Configuration,
    DocumentSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new DocumentsApi(configuration);

let workspaceId: string; // (default to undefined)
let documentSearchRequest: DocumentSearchRequest; //

const { status, data } = await apiInstance.searchDocuments(
    workspaceId,
    documentSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **documentSearchRequest** | **DocumentSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<DocumentResponse>**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **searchFaqs**
> Array<FaqResponse> searchFaqs(faqSearchRequest)


### Example

```typescript
import {
    DocumentsApi,
    Configuration,
    FaqSearchRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new DocumentsApi(configuration);

let workspaceId: string; // (default to undefined)
let faqSearchRequest: FaqSearchRequest; //

const { status, data } = await apiInstance.searchFaqs(
    workspaceId,
    faqSearchRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **faqSearchRequest** | **FaqSearchRequest**|  | |
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<FaqResponse>**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateDocument**
> DocumentResponse updateDocument(documentUpdateRequest)


### Example

```typescript
import {
    DocumentsApi,
    Configuration,
    DocumentUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new DocumentsApi(configuration);

let docId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let documentUpdateRequest: DocumentUpdateRequest; //

const { status, data } = await apiInstance.updateDocument(
    docId,
    workspaceId,
    documentUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **documentUpdateRequest** | **DocumentUpdateRequest**|  | |
| **docId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**DocumentResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateDocumentCategory**
> DocumentCategoryResponse updateDocumentCategory(documentCategoryUpdateRequest)


### Example

```typescript
import {
    DocumentsApi,
    Configuration,
    DocumentCategoryUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new DocumentsApi(configuration);

let catId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let documentCategoryUpdateRequest: DocumentCategoryUpdateRequest; //

const { status, data } = await apiInstance.updateDocumentCategory(
    catId,
    workspaceId,
    documentCategoryUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **documentCategoryUpdateRequest** | **DocumentCategoryUpdateRequest**|  | |
| **catId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**DocumentCategoryResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateFaq**
> Array<FaqResponse> updateFaq(faqUpdateRequest)


### Example

```typescript
import {
    DocumentsApi,
    Configuration,
    FaqUpdateRequest
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new DocumentsApi(configuration);

let faqId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let faqUpdateRequest: FaqUpdateRequest; //

const { status, data } = await apiInstance.updateFaq(
    faqId,
    workspaceId,
    faqUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **faqUpdateRequest** | **FaqUpdateRequest**|  | |
| **faqId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<FaqResponse>**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **uploadFromUrlDocument**
> DocumentResponse uploadFromUrlDocument(appUrlInput)


### Example

```typescript
import {
    DocumentsApi,
    Configuration,
    AppUrlInput
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new DocumentsApi(configuration);

let catId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let appUrlInput: AppUrlInput; //

const { status, data } = await apiInstance.uploadFromUrlDocument(
    catId,
    workspaceId,
    appUrlInput
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appUrlInput** | **AppUrlInput**|  | |
| **catId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|


### Return type

**DocumentResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **uploadMemoryDocument**
> DocumentResponse uploadMemoryDocument()


### Example

```typescript
import {
    DocumentsApi,
    Configuration
} from 'flowhunt';

const configuration = new Configuration();
const apiInstance = new DocumentsApi(configuration);

let catId: string; // (default to undefined)
let workspaceId: string; // (default to undefined)
let file: File; // (default to undefined)

const { status, data } = await apiInstance.uploadMemoryDocument(
    catId,
    workspaceId,
    file
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **catId** | [**string**] |  | defaults to undefined|
| **workspaceId** | [**string**] |  | defaults to undefined|
| **file** | [**File**] |  | defaults to undefined|


### Return type

**DocumentResponse**

### Authorization

[APIKeyHeader](../README.md#APIKeyHeader), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

