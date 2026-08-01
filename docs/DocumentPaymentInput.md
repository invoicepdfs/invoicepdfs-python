# DocumentPaymentInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bank_account** | [**InvoiceBankAccountInput**](InvoiceBankAccountInput.md) |  | [optional] 
**payment_url** | **str** |  | [optional] 
**accepted_methods** | **List[str]** |  | [optional] 
**instructions** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.document_payment_input import DocumentPaymentInput

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentPaymentInput from a JSON string
document_payment_input_instance = DocumentPaymentInput.from_json(json)
# print the JSON string representation of the object
print(DocumentPaymentInput.to_json())

# convert the object into a dict
document_payment_input_dict = document_payment_input_instance.to_dict()
# create an instance of DocumentPaymentInput from a dict
document_payment_input_from_dict = DocumentPaymentInput.from_dict(document_payment_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


