# DocumentPartyInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**legal_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**phone** | **str** |  | [optional] 
**website** | **str** |  | [optional] 
**tax_id** | **str** |  | [optional] 
**registration_number** | **str** |  | [optional] 
**address** | [**PostalAddress**](PostalAddress.md) |  | [optional] 
**bank_account** | [**InvoiceBankAccountInput**](InvoiceBankAccountInput.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.document_party_input import DocumentPartyInput

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentPartyInput from a JSON string
document_party_input_instance = DocumentPartyInput.from_json(json)
# print the JSON string representation of the object
print(DocumentPartyInput.to_json())

# convert the object into a dict
document_party_input_dict = document_party_input_instance.to_dict()
# create an instance of DocumentPartyInput from a dict
document_party_input_from_dict = DocumentPartyInput.from_dict(document_party_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


