# AuthRefreshResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AuthRefreshData**](AuthRefreshData.md) |  | 

## Example

```python
from invoicepdfs.models.auth_refresh_response import AuthRefreshResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AuthRefreshResponse from a JSON string
auth_refresh_response_instance = AuthRefreshResponse.from_json(json)
# print the JSON string representation of the object
print(AuthRefreshResponse.to_json())

# convert the object into a dict
auth_refresh_response_dict = auth_refresh_response_instance.to_dict()
# create an instance of AuthRefreshResponse from a dict
auth_refresh_response_from_dict = AuthRefreshResponse.from_dict(auth_refresh_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


