# DocumentShippingInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** |  | [optional] [default to 'Shipping']
**amount** | **str** |  | 

## Example

```python
from invoicepdfs.models.document_shipping_input import DocumentShippingInput

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentShippingInput from a JSON string
document_shipping_input_instance = DocumentShippingInput.from_json(json)
# print the JSON string representation of the object
print(DocumentShippingInput.to_json())

# convert the object into a dict
document_shipping_input_dict = document_shipping_input_instance.to_dict()
# create an instance of DocumentShippingInput from a dict
document_shipping_input_from_dict = DocumentShippingInput.from_dict(document_shipping_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


