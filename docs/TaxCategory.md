# TaxCategory

How a tax is treated, as opposed to what it is called.  `name` and `rate` do not say this: two taxes at 0% may be zero-rated, exempt, reverse-charge or outside scope, and EN 16931 keeps them in separate VAT breakdown groups with different mandatory fields. Optional, so an invoice that never mentions a category calculates exactly as before.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** | UNCL5305 tax category code — S standard, Z zero-rated, E exempt, AE reverse charge, K intra-community, G export, O outside scope | 
**exemption_reason** | **str** |  | [optional] 
**exemption_reason_code** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.tax_category import TaxCategory

# TODO update the JSON string below
json = "{}"
# create an instance of TaxCategory from a JSON string
tax_category_instance = TaxCategory.from_json(json)
# print the JSON string representation of the object
print(TaxCategory.to_json())

# convert the object into a dict
tax_category_dict = tax_category_instance.to_dict()
# create an instance of TaxCategory from a dict
tax_category_from_dict = TaxCategory.from_dict(tax_category_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


