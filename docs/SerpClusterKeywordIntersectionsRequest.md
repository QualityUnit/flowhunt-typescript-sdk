# SerpClusterKeywordIntersectionsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**keyword_id** | **string** |  | [optional] [default to undefined]
**keyword** | **string** | Keyword to search | [default to undefined]
**language** | **string** |  | [optional] [default to undefined]
**country** | **string** |  | [optional] [default to undefined]
**search_engine** | [**SerpSearchEngineType**](SerpSearchEngineType.md) |  | [optional] [default to undefined]
**customer_id** | **string** | Customer ID of cluster | [default to undefined]
**campaign_id** | **string** |  | [optional] [default to undefined]
**group_id** | **string** |  | [optional] [default to undefined]
**min_cluster_strength** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { SerpClusterKeywordIntersectionsRequest } from 'flowhunt';

const instance: SerpClusterKeywordIntersectionsRequest = {
    keyword_id,
    keyword,
    language,
    country,
    search_engine,
    customer_id,
    campaign_id,
    group_id,
    min_cluster_strength,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
