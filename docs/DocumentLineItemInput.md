# DocumentLineItemInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**description** | **str** |  | [optional] 
**quantity** | **str** |  | 
**unit_price** | **str** | Decimal string in major units | 
**unit** | **str** |  | [optional] 
**sku** | **str** |  | [optional] 
**discount** | [**DocumentDiscountInput**](DocumentDiscountInput.md) |  | [optional] 
**taxes** | [**List[DocumentLineItemTaxInput]**](DocumentLineItemTaxInput.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.document_line_item_input import DocumentLineItemInput

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentLineItemInput from a JSON string
document_line_item_input_instance = DocumentLineItemInput.from_json(json)
# print the JSON string representation of the object
print(DocumentLineItemInput.to_json())

# convert the object into a dict
document_line_item_input_dict = document_line_item_input_instance.to_dict()
# create an instance of DocumentLineItemInput from a dict
document_line_item_input_from_dict = DocumentLineItemInput.from_dict(document_line_item_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


