# InvoiceBankAccountInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bank_name** | **str** |  | [optional] 
**account_name** | **str** |  | [optional] 
**account_number** | **str** |  | [optional] 
**routing_number** | **str** |  | [optional] 
**swift** | **str** |  | [optional] 
**iban** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.invoice_bank_account_input import InvoiceBankAccountInput

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceBankAccountInput from a JSON string
invoice_bank_account_input_instance = InvoiceBankAccountInput.from_json(json)
# print the JSON string representation of the object
print(InvoiceBankAccountInput.to_json())

# convert the object into a dict
invoice_bank_account_input_dict = invoice_bank_account_input_instance.to_dict()
# create an instance of InvoiceBankAccountInput from a dict
invoice_bank_account_input_from_dict = InvoiceBankAccountInput.from_dict(invoice_bank_account_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


