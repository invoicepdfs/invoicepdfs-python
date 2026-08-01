# BrandingResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BrandingOut**](BrandingOut.md) |  | 

## Example

```python
from invoicepdfs.models.branding_response import BrandingResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BrandingResponse from a JSON string
branding_response_instance = BrandingResponse.from_json(json)
# print the JSON string representation of the object
print(BrandingResponse.to_json())

# convert the object into a dict
branding_response_dict = branding_response_instance.to_dict()
# create an instance of BrandingResponse from a dict
branding_response_from_dict = BrandingResponse.from_dict(branding_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


