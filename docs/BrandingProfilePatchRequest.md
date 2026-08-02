# BrandingProfilePatchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**primary_color** | **str** |  | [optional] 
**accent_color** | **str** |  | [optional] 
**font_family** | **str** |  | [optional] 
**header_text** | **str** |  | [optional] 
**footer_text** | **str** |  | [optional] 
**hide_invoicepdfs_branding** | **bool** |  | [optional] 
**is_default** | **bool** |  | [optional] 

## Example

```python
from invoicepdfs.models.branding_profile_patch_request import BrandingProfilePatchRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BrandingProfilePatchRequest from a JSON string
branding_profile_patch_request_instance = BrandingProfilePatchRequest.from_json(json)
# print the JSON string representation of the object
print(BrandingProfilePatchRequest.to_json())

# convert the object into a dict
branding_profile_patch_request_dict = branding_profile_patch_request_instance.to_dict()
# create an instance of BrandingProfilePatchRequest from a dict
branding_profile_patch_request_from_dict = BrandingProfilePatchRequest.from_dict(branding_profile_patch_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


