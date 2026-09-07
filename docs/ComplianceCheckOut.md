# ComplianceCheckOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**profile** | **str** |  | 
**ruleset_version** | **str** | The version these rules came from. Worth recording alongside any document you file — rulesets revise, and &#39;which rules did this pass?&#39; is what an audit asks years later. | 
**valid** | **bool** |  | 
**violations** | [**List[ComplianceViolationOut]**](ComplianceViolationOut.md) | Every violation found, not the first — fixing one field per round trip is the experience this avoids. | [optional] 

## Example

```python
from invoicepdfs.models.compliance_check_out import ComplianceCheckOut

# TODO update the JSON string below
json = "{}"
# create an instance of ComplianceCheckOut from a JSON string
compliance_check_out_instance = ComplianceCheckOut.from_json(json)
# print the JSON string representation of the object
print(ComplianceCheckOut.to_json())

# convert the object into a dict
compliance_check_out_dict = compliance_check_out_instance.to_dict()
# create an instance of ComplianceCheckOut from a dict
compliance_check_out_from_dict = ComplianceCheckOut.from_dict(compliance_check_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


