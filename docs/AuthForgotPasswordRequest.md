# AuthForgotPasswordRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** | Email address of the account | 

## Example

```python
from invoicepdfs.models.auth_forgot_password_request import AuthForgotPasswordRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AuthForgotPasswordRequest from a JSON string
auth_forgot_password_request_instance = AuthForgotPasswordRequest.from_json(json)
# print the JSON string representation of the object
print(AuthForgotPasswordRequest.to_json())

# convert the object into a dict
auth_forgot_password_request_dict = auth_forgot_password_request_instance.to_dict()
# create an instance of AuthForgotPasswordRequest from a dict
auth_forgot_password_request_from_dict = AuthForgotPasswordRequest.from_dict(auth_forgot_password_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


