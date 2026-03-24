# GoogleAdsKeywordAddRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customer_id** | **string** | Customer id | [default to undefined]
**campaign_id** | **string** | Campaign id | [default to undefined]
**group_id** | **string** | Group id | [default to undefined]
**keywords** | **Array&lt;string&gt;** | List of keywords to add | [default to undefined]
**is_negative** | **boolean** | Is negative keyword | [optional] [default to false]
**match_type** | [**GoogleAdsMatchType**](GoogleAdsMatchType.md) | Match type | [default to undefined]

## Example

```typescript
import { GoogleAdsKeywordAddRequest } from 'flowhunt';

const instance: GoogleAdsKeywordAddRequest = {
    customer_id,
    campaign_id,
    group_id,
    keywords,
    is_negative,
    match_type,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
