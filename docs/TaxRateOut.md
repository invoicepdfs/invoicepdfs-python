# TaxRateOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**name** | **str** |  | 
**rate** | **str** |  | 
**inclusive** | **bool** |  | 
**jurisdiction** | **str** |  | [optional] 
**is_active** | **bool** |  | 
**created_at** | **str** |  | 
**updated_at** | **str** |  | 

## Example

```python
from invoicepdfs.models.tax_rate_out import TaxRateOut

# TODO update the JSON string below
json = "{}"
# create an instance of TaxRateOut from a JSON string
tax_rate_out_instance = TaxRateOut.from_json(json)
# print the JSON string representation of the object
print(TaxRateOut.to_json())

# convert the object into a dict
tax_rate_out_dict = tax_rate_out_instance.to_dict()
# create an instance of TaxRateOut from a dict
tax_rate_out_from_dict = TaxRateOut.from_dict(tax_rate_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


