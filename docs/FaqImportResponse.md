# FaqImportResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**successful** | [**Array&lt;FaqResponse&gt;**](FaqResponse.md) | List of successfully imported FAQs | [default to undefined]
**failed** | [**Array&lt;FailedFaqItem&gt;**](FailedFaqItem.md) | List of FAQs that failed to import | [default to undefined]
**total_attempted** | **number** | Total number of FAQs attempted | [default to undefined]
**total_successful** | **number** | Number of successfully imported FAQs | [default to undefined]
**total_failed** | **number** | Number of failed FAQs | [default to undefined]

## Example

```typescript
import { FaqImportResponse } from 'flowhunt';

const instance: FaqImportResponse = {
    successful,
    failed,
    total_attempted,
    total_successful,
    total_failed,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
