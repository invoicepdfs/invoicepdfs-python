# ComplianceViolationOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**rule** | **str** | The EN 16931 term or group. | 
**path** | **str** | Where in the document. | 
**message** | **str** |  | 

## Example

```python
from invoicepdfs.models.compliance_violation_out import ComplianceViolationOut

# TODO update the JSON string below
json = "{}"
# create an instance of ComplianceViolationOut from a JSON string
compliance_violation_out_instance = ComplianceViolationOut.from_json(json)
# print the JSON string representation of the object
print(ComplianceViolationOut.to_json())

# convert the object into a dict
compliance_violation_out_dict = compliance_violation_out_instance.to_dict()
# create an instance of ComplianceViolationOut from a dict
compliance_violation_out_from_dict = ComplianceViolationOut.from_dict(compliance_violation_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


