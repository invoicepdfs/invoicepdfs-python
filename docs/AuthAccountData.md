# AuthAccountData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | 
**name** | **str** |  | 
**email** | **str** |  | [optional] 
**plan_id** | **str** |  | 
**plan_name** | **str** |  | 

## Example

```python
from invoicepdfs.models.auth_account_data import AuthAccountData

# TODO update the JSON string below
json = "{}"
# create an instance of AuthAccountData from a JSON string
auth_account_data_instance = AuthAccountData.from_json(json)
# print the JSON string representation of the object
print(AuthAccountData.to_json())

# convert the object into a dict
auth_account_data_dict = auth_account_data_instance.to_dict()
# create an instance of AuthAccountData from a dict
auth_account_data_from_dict = AuthAccountData.from_dict(auth_account_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


