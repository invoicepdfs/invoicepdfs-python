# ApiKeyPatchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 

## Example

```python
from invoicepdfs.models.api_key_patch_request import ApiKeyPatchRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ApiKeyPatchRequest from a JSON string
api_key_patch_request_instance = ApiKeyPatchRequest.from_json(json)
# print the JSON string representation of the object
print(ApiKeyPatchRequest.to_json())

# convert the object into a dict
api_key_patch_request_dict = api_key_patch_request_instance.to_dict()
# create an instance of ApiKeyPatchRequest from a dict
api_key_patch_request_from_dict = ApiKeyPatchRequest.from_dict(api_key_patch_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


