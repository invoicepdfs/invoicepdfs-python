# AuthRegisterResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AuthAccountData**](AuthAccountData.md) |  | 

## Example

```python
from invoicepdfs.models.auth_register_response import AuthRegisterResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AuthRegisterResponse from a JSON string
auth_register_response_instance = AuthRegisterResponse.from_json(json)
# print the JSON string representation of the object
print(AuthRegisterResponse.to_json())

# convert the object into a dict
auth_register_response_dict = auth_register_response_instance.to_dict()
# create an instance of AuthRegisterResponse from a dict
auth_register_response_from_dict = AuthRegisterResponse.from_dict(auth_register_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


