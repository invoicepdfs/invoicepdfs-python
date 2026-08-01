# InvoicePaymentInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bank_account** | [**InvoiceBankAccountInput**](InvoiceBankAccountInput.md) |  | [optional] 
**payment_url** | **str** |  | [optional] 
**accepted_methods** | **List[str]** |  | [optional] 
**instructions** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.invoice_payment_input import InvoicePaymentInput

# TODO update the JSON string below
json = "{}"
# create an instance of InvoicePaymentInput from a JSON string
invoice_payment_input_instance = InvoicePaymentInput.from_json(json)
# print the JSON string representation of the object
print(InvoicePaymentInput.to_json())

# convert the object into a dict
invoice_payment_input_dict = invoice_payment_input_instance.to_dict()
# create an instance of InvoicePaymentInput from a dict
invoice_payment_input_from_dict = InvoicePaymentInput.from_dict(invoice_payment_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


