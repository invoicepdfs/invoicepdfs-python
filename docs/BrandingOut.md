# BrandingOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**logo_file_id** | **str** |  | [optional] 
**primary_color** | **str** |  | 
**accent_color** | **str** |  | 
**font_family** | **str** |  | [optional] 
**footer_text** | **str** |  | 
**hide_invoicepdfs_branding** | **bool** |  | 
**created_at** | **str** |  | 
**updated_at** | **str** |  | 

## Example

```python
from invoicepdfs.models.branding_out import BrandingOut

# TODO update the JSON string below
json = "{}"
# create an instance of BrandingOut from a JSON string
branding_out_instance = BrandingOut.from_json(json)
# print the JSON string representation of the object
print(BrandingOut.to_json())

# convert the object into a dict
branding_out_dict = branding_out_instance.to_dict()
# create an instance of BrandingOut from a dict
branding_out_from_dict = BrandingOut.from_dict(branding_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


