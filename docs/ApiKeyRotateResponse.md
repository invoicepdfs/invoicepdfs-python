# ApiKeyRotateResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**ApiKeyCreated**](ApiKeyCreated.md) |  | 

## Example

```python
from invoicepdfs.models.api_key_rotate_response import ApiKeyRotateResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ApiKeyRotateResponse from a JSON string
api_key_rotate_response_instance = ApiKeyRotateResponse.from_json(json)
# print the JSON string representation of the object
print(ApiKeyRotateResponse.to_json())

# convert the object into a dict
api_key_rotate_response_dict = api_key_rotate_response_instance.to_dict()
# create an instance of ApiKeyRotateResponse from a dict
api_key_rotate_response_from_dict = ApiKeyRotateResponse.from_dict(api_key_rotate_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


