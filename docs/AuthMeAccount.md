# AuthMeAccount


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**name** | **str** |  | 
**plan_id** | **str** |  | 
**plan_name** | **str** |  | 

## Example

```python
from invoicepdfs.models.auth_me_account import AuthMeAccount

# TODO update the JSON string below
json = "{}"
# create an instance of AuthMeAccount from a JSON string
auth_me_account_instance = AuthMeAccount.from_json(json)
# print the JSON string representation of the object
print(AuthMeAccount.to_json())

# convert the object into a dict
auth_me_account_dict = auth_me_account_instance.to_dict()
# create an instance of AuthMeAccount from a dict
auth_me_account_from_dict = AuthMeAccount.from_dict(auth_me_account_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


