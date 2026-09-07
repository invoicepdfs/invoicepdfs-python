# DocumentComplianceRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**document_type** | **str** |  | [optional] [default to 'invoice']
**data** | [**DocumentInvoiceDataInput**](DocumentInvoiceDataInput.md) |  | 
**profile** | **str** | Which ruleset to hold the document to. Rulesets differ: a document valid under one can be rejected by another, so there is no default. | 

## Example

```python
from invoicepdfs.models.document_compliance_request import DocumentComplianceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentComplianceRequest from a JSON string
document_compliance_request_instance = DocumentComplianceRequest.from_json(json)
# print the JSON string representation of the object
print(DocumentComplianceRequest.to_json())

# convert the object into a dict
document_compliance_request_dict = document_compliance_request_instance.to_dict()
# create an instance of DocumentComplianceRequest from a dict
document_compliance_request_from_dict = DocumentComplianceRequest.from_dict(document_compliance_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


