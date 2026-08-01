# BusinessProfileResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BusinessProfileOut**](BusinessProfileOut.md) |  | 

## Example

```python
from invoicepdfs.models.business_profile_response import BusinessProfileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BusinessProfileResponse from a JSON string
business_profile_response_instance = BusinessProfileResponse.from_json(json)
# print the JSON string representation of the object
print(BusinessProfileResponse.to_json())

# convert the object into a dict
business_profile_response_dict = business_profile_response_instance.to_dict()
# create an instance of BusinessProfileResponse from a dict
business_profile_response_from_dict = BusinessProfileResponse.from_dict(business_profile_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


