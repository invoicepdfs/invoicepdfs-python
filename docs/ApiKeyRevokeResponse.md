# ApiKeyRevokeResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | **Dict[str, bool]** |  | 

## Example

```python
from invoicepdfs.models.api_key_revoke_response import ApiKeyRevokeResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ApiKeyRevokeResponse from a JSON string
api_key_revoke_response_instance = ApiKeyRevokeResponse.from_json(json)
# print the JSON string representation of the object
print(ApiKeyRevokeResponse.to_json())

# convert the object into a dict
api_key_revoke_response_dict = api_key_revoke_response_instance.to_dict()
# create an instance of ApiKeyRevokeResponse from a dict
api_key_revoke_response_from_dict = ApiKeyRevokeResponse.from_dict(api_key_revoke_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


