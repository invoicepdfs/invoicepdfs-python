# AuthMeData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account** | [**AuthMeAccount**](AuthMeAccount.md) |  | 

## Example

```python
from invoicepdfs.models.auth_me_data import AuthMeData

# TODO update the JSON string below
json = "{}"
# create an instance of AuthMeData from a JSON string
auth_me_data_instance = AuthMeData.from_json(json)
# print the JSON string representation of the object
print(AuthMeData.to_json())

# convert the object into a dict
auth_me_data_dict = auth_me_data_instance.to_dict()
# create an instance of AuthMeData from a dict
auth_me_data_from_dict = AuthMeData.from_dict(auth_me_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


