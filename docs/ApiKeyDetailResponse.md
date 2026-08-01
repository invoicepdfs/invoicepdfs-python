# ApiKeyDetailResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**ApiKeyListItem**](ApiKeyListItem.md) |  | 

## Example

```python
from invoicepdfs.models.api_key_detail_response import ApiKeyDetailResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ApiKeyDetailResponse from a JSON string
api_key_detail_response_instance = ApiKeyDetailResponse.from_json(json)
# print the JSON string representation of the object
print(ApiKeyDetailResponse.to_json())

# convert the object into a dict
api_key_detail_response_dict = api_key_detail_response_instance.to_dict()
# create an instance of ApiKeyDetailResponse from a dict
api_key_detail_response_from_dict = ApiKeyDetailResponse.from_dict(api_key_detail_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


