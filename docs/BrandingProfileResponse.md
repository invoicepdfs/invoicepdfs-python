# BrandingProfileResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BrandingProfileOut**](BrandingProfileOut.md) |  | 

## Example

```python
from invoicepdfs.models.branding_profile_response import BrandingProfileResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BrandingProfileResponse from a JSON string
branding_profile_response_instance = BrandingProfileResponse.from_json(json)
# print the JSON string representation of the object
print(BrandingProfileResponse.to_json())

# convert the object into a dict
branding_profile_response_dict = branding_profile_response_instance.to_dict()
# create an instance of BrandingProfileResponse from a dict
branding_profile_response_from_dict = BrandingProfileResponse.from_dict(branding_profile_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


