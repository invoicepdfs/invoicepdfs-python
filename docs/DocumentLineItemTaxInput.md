# DocumentLineItemTaxInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**rate** | **str** |  | 
**inclusive** | **bool** |  | [optional] [default to False]

## Example

```python
from invoicepdfs.models.document_line_item_tax_input import DocumentLineItemTaxInput

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentLineItemTaxInput from a JSON string
document_line_item_tax_input_instance = DocumentLineItemTaxInput.from_json(json)
# print the JSON string representation of the object
print(DocumentLineItemTaxInput.to_json())

# convert the object into a dict
document_line_item_tax_input_dict = document_line_item_tax_input_instance.to_dict()
# create an instance of DocumentLineItemTaxInput from a dict
document_line_item_tax_input_from_dict = DocumentLineItemTaxInput.from_dict(document_line_item_tax_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


