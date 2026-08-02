# BrandingProfileOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**name** | **str** |  | 
**is_default** | **bool** |  | 
**logo_file_id** | **str** |  | [optional] 
**primary_color** | **str** |  | 
**accent_color** | **str** |  | 
**font_family** | **str** |  | [optional] 
**header_text** | **str** |  | [optional] 
**footer_text** | **str** |  | 
**hide_invoicepdfs_branding** | **bool** |  | 
**created_at** | **str** |  | 
**updated_at** | **str** |  | 

## Example

```python
from invoicepdfs.models.branding_profile_out import BrandingProfileOut

# TODO update the JSON string below
json = "{}"
# create an instance of BrandingProfileOut from a JSON string
branding_profile_out_instance = BrandingProfileOut.from_json(json)
# print the JSON string representation of the object
print(BrandingProfileOut.to_json())

# convert the object into a dict
branding_profile_out_dict = branding_profile_out_instance.to_dict()
# create an instance of BrandingProfileOut from a dict
branding_profile_out_from_dict = BrandingProfileOut.from_dict(branding_profile_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


