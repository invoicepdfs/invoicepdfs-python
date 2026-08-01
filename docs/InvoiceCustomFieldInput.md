# InvoiceCustomFieldInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**label** | **str** |  | 
**value** | **str** |  | 

## Example

```python
from invoicepdfs.models.invoice_custom_field_input import InvoiceCustomFieldInput

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceCustomFieldInput from a JSON string
invoice_custom_field_input_instance = InvoiceCustomFieldInput.from_json(json)
# print the JSON string representation of the object
print(InvoiceCustomFieldInput.to_json())

# convert the object into a dict
invoice_custom_field_input_dict = invoice_custom_field_input_instance.to_dict()
# create an instance of InvoiceCustomFieldInput from a dict
invoice_custom_field_input_from_dict = InvoiceCustomFieldInput.from_dict(invoice_custom_field_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


