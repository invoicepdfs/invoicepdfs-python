# DocumentComplianceResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**ComplianceCheckOut**](ComplianceCheckOut.md) |  | 

## Example

```python
from invoicepdfs.models.document_compliance_response import DocumentComplianceResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentComplianceResponse from a JSON string
document_compliance_response_instance = DocumentComplianceResponse.from_json(json)
# print the JSON string representation of the object
print(DocumentComplianceResponse.to_json())

# convert the object into a dict
document_compliance_response_dict = document_compliance_response_instance.to_dict()
# create an instance of DocumentComplianceResponse from a dict
document_compliance_response_from_dict = DocumentComplianceResponse.from_dict(document_compliance_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


