# StandardLineItemInput

A fully priced line: unit, price, tax, discount and SKU.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**description** | **str** |  | [optional] 
**quantity** | **str** | Decimal string | 
**unit_price** | **str** | Decimal string, major units | [optional] [default to '0.00']
**unit** | **str** |  | [optional] 
**sku** | **str** |  | [optional] 
**discount** | [**LineItemDiscountInput**](LineItemDiscountInput.md) |  | [optional] 
**taxes** | [**List[LineItemTaxInput]**](LineItemTaxInput.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.standard_line_item_input import StandardLineItemInput

# TODO update the JSON string below
json = "{}"
# create an instance of StandardLineItemInput from a JSON string
standard_line_item_input_instance = StandardLineItemInput.from_json(json)
# print the JSON string representation of the object
print(StandardLineItemInput.to_json())

# convert the object into a dict
standard_line_item_input_dict = standard_line_item_input_instance.to_dict()
# create an instance of StandardLineItemInput from a dict
standard_line_item_input_from_dict = StandardLineItemInput.from_dict(standard_line_item_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


