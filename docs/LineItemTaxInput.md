# LineItemTaxInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tax_rate_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**rate** | **str** |  | [optional] 
**inclusive** | **bool** |  | [optional] [default to False]

## Example

```python
from invoicepdfs.models.line_item_tax_input import LineItemTaxInput

# TODO update the JSON string below
json = "{}"
# create an instance of LineItemTaxInput from a JSON string
line_item_tax_input_instance = LineItemTaxInput.from_json(json)
# print the JSON string representation of the object
print(LineItemTaxInput.to_json())

# convert the object into a dict
line_item_tax_input_dict = line_item_tax_input_instance.to_dict()
# create an instance of LineItemTaxInput from a dict
line_item_tax_input_from_dict = LineItemTaxInput.from_dict(line_item_tax_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


