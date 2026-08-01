# TaxRatePatchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**rate** | **str** |  | [optional] 
**inclusive** | **bool** |  | [optional] 
**jurisdiction** | **str** |  | [optional] 
**is_active** | **bool** |  | [optional] 

## Example

```python
from invoicepdfs.models.tax_rate_patch_request import TaxRatePatchRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TaxRatePatchRequest from a JSON string
tax_rate_patch_request_instance = TaxRatePatchRequest.from_json(json)
# print the JSON string representation of the object
print(TaxRatePatchRequest.to_json())

# convert the object into a dict
tax_rate_patch_request_dict = tax_rate_patch_request_instance.to_dict()
# create an instance of TaxRatePatchRequest from a dict
tax_rate_patch_request_from_dict = TaxRatePatchRequest.from_dict(tax_rate_patch_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


