# ElectronicAddress

BT-34 / BT-49 — where a document is routed on Peppol or DBNA.  Both halves are required: an identifier without its scheme cannot be resolved, because the same string means different things in different code lists. This is not the tax id, which identifies a company to a tax authority rather than a mailbox on a network.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **str** |  | 
**scheme_id** | **str** | EAS code list identifier — 0088 is GLN, 9930 a German VAT number. | 

## Example

```python
from invoicepdfs.models.electronic_address import ElectronicAddress

# TODO update the JSON string below
json = "{}"
# create an instance of ElectronicAddress from a JSON string
electronic_address_instance = ElectronicAddress.from_json(json)
# print the JSON string representation of the object
print(ElectronicAddress.to_json())

# convert the object into a dict
electronic_address_dict = electronic_address_instance.to_dict()
# create an instance of ElectronicAddress from a dict
electronic_address_from_dict = ElectronicAddress.from_dict(electronic_address_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


