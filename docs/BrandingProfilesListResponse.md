# BrandingProfilesListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BrandingProfileOut]**](BrandingProfileOut.md) |  | 

## Example

```python
from invoicepdfs.models.branding_profiles_list_response import BrandingProfilesListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BrandingProfilesListResponse from a JSON string
branding_profiles_list_response_instance = BrandingProfilesListResponse.from_json(json)
# print the JSON string representation of the object
print(BrandingProfilesListResponse.to_json())

# convert the object into a dict
branding_profiles_list_response_dict = branding_profiles_list_response_instance.to_dict()
# create an instance of BrandingProfilesListResponse from a dict
branding_profiles_list_response_from_dict = BrandingProfilesListResponse.from_dict(branding_profiles_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


