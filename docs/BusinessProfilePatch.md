# BusinessProfilePatch


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**legal_name** | **str** |  | [optional] 
**display_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**phone** | **str** |  | [optional] 
**website** | **str** |  | [optional] 
**tax_id** | **str** |  | [optional] 
**address** | [**PostalAddress**](PostalAddress.md) |  | [optional] 
**default_currency** | **str** |  | [optional] 
**default_locale** | **str** |  | [optional] 
**default_timezone** | **str** |  | [optional] 
**logo_file_id** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.business_profile_patch import BusinessProfilePatch

# TODO update the JSON string below
json = "{}"
# create an instance of BusinessProfilePatch from a JSON string
business_profile_patch_instance = BusinessProfilePatch.from_json(json)
# print the JSON string representation of the object
print(BusinessProfilePatch.to_json())

# convert the object into a dict
business_profile_patch_dict = business_profile_patch_instance.to_dict()
# create an instance of BusinessProfilePatch from a dict
business_profile_patch_from_dict = BusinessProfilePatch.from_dict(business_profile_patch_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


