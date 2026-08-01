# AuthMePatchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.auth_me_patch_request import AuthMePatchRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AuthMePatchRequest from a JSON string
auth_me_patch_request_instance = AuthMePatchRequest.from_json(json)
# print the JSON string representation of the object
print(AuthMePatchRequest.to_json())

# convert the object into a dict
auth_me_patch_request_dict = auth_me_patch_request_instance.to_dict()
# create an instance of AuthMePatchRequest from a dict
auth_me_patch_request_from_dict = AuthMePatchRequest.from_dict(auth_me_patch_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


