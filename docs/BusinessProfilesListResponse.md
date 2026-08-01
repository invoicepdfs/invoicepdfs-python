# BusinessProfilesListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BusinessProfileOut]**](BusinessProfileOut.md) |  | 
**pagination** | [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.business_profiles_list_response import BusinessProfilesListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BusinessProfilesListResponse from a JSON string
business_profiles_list_response_instance = BusinessProfilesListResponse.from_json(json)
# print the JSON string representation of the object
print(BusinessProfilesListResponse.to_json())

# convert the object into a dict
business_profiles_list_response_dict = business_profiles_list_response_instance.to_dict()
# create an instance of BusinessProfilesListResponse from a dict
business_profiles_list_response_from_dict = BusinessProfilesListResponse.from_dict(business_profiles_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


