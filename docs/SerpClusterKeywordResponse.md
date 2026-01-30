# SerpClusterKeywordResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**unique_id** | **string** | Unique ID | [default to undefined]
**keyword_id** | **string** | Query ID | [default to undefined]
**keyword** | **string** | Query | [default to undefined]
**country** | **string** |  | [optional] [default to undefined]
**language** | **string** |  | [optional] [default to undefined]
**is_negative** | **boolean** |  | [optional] [default to undefined]
**match_type** | [**GoogleAdsMatchType**](GoogleAdsMatchType.md) |  | [default to undefined]
**campaign_id** | **string** | Campaign ID | [default to undefined]
**group_id** | **string** | Group ID | [default to undefined]
**search_engine** | [**SerpSearchEngineType**](SerpSearchEngineType.md) |  | [default to undefined]

## Example

```typescript
import { SerpClusterKeywordResponse } from 'flowhunt';

const instance: SerpClusterKeywordResponse = {
    unique_id,
    keyword_id,
    keyword,
    country,
    language,
    is_negative,
    match_type,
    campaign_id,
    group_id,
    search_engine,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
