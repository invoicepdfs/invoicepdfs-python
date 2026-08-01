# AuthResetPasswordRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**oob_code** | **str** | Code from the password reset email | 
**new_password** | **str** | New password | 

## Example

```python
from invoicepdfs.models.auth_reset_password_request import AuthResetPasswordRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AuthResetPasswordRequest from a JSON string
auth_reset_password_request_instance = AuthResetPasswordRequest.from_json(json)
# print the JSON string representation of the object
print(AuthResetPasswordRequest.to_json())

# convert the object into a dict
auth_reset_password_request_dict = auth_reset_password_request_instance.to_dict()
# create an instance of AuthResetPasswordRequest from a dict
auth_reset_password_request_from_dict = AuthResetPasswordRequest.from_dict(auth_reset_password_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


