# InvoiceTermInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**content** | **str** |  | 

## Example

```python
from invoicepdfs.models.invoice_term_input import InvoiceTermInput

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceTermInput from a JSON string
invoice_term_input_instance = InvoiceTermInput.from_json(json)
# print the JSON string representation of the object
print(InvoiceTermInput.to_json())

# convert the object into a dict
invoice_term_input_dict = invoice_term_input_instance.to_dict()
# create an instance of InvoiceTermInput from a dict
invoice_term_input_from_dict = InvoiceTermInput.from_dict(invoice_term_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


