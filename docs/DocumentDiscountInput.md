# DocumentDiscountInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] [default to 'percentage']
**value** | **str** |  | 
**reason** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.document_discount_input import DocumentDiscountInput

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentDiscountInput from a JSON string
document_discount_input_instance = DocumentDiscountInput.from_json(json)
# print the JSON string representation of the object
print(DocumentDiscountInput.to_json())

# convert the object into a dict
document_discount_input_dict = document_discount_input_instance.to_dict()
# create an instance of DocumentDiscountInput from a dict
document_discount_input_from_dict = DocumentDiscountInput.from_dict(document_discount_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


