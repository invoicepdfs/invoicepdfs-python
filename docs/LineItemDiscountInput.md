# LineItemDiscountInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] [default to 'percentage']
**value** | **str** |  | 
**reason** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.line_item_discount_input import LineItemDiscountInput

# TODO update the JSON string below
json = "{}"
# create an instance of LineItemDiscountInput from a JSON string
line_item_discount_input_instance = LineItemDiscountInput.from_json(json)
# print the JSON string representation of the object
print(LineItemDiscountInput.to_json())

# convert the object into a dict
line_item_discount_input_dict = line_item_discount_input_instance.to_dict()
# create an instance of LineItemDiscountInput from a dict
line_item_discount_input_from_dict = LineItemDiscountInput.from_dict(line_item_discount_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


