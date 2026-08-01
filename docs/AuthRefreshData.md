# AuthRefreshData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id_token** | **str** |  | 
**refresh_token** | **str** |  | 
**expires_in** | **int** |  | 

## Example

```python
from invoicepdfs.models.auth_refresh_data import AuthRefreshData

# TODO update the JSON string below
json = "{}"
# create an instance of AuthRefreshData from a JSON string
auth_refresh_data_instance = AuthRefreshData.from_json(json)
# print the JSON string representation of the object
print(AuthRefreshData.to_json())

# convert the object into a dict
auth_refresh_data_dict = auth_refresh_data_instance.to_dict()
# create an instance of AuthRefreshData from a dict
auth_refresh_data_from_dict = AuthRefreshData.from_dict(auth_refresh_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


