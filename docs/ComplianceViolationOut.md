# ComplianceViolationOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**rule** | **str** | The identifier the standard uses — a business term from the mandatory-field check, a rule id from Schematron. A rule id is what a rejection notice from an access point quotes. | 
**path** | **str** | Where the problem is. The mandatory-field check names a field of the request; Schematron names the node in the generated XML. | 
**message** | **str** |  | 
**severity** | **str** | &#x60;fatal&#x60; would get the document rejected. &#x60;warning&#x60; is a recommendation — both EN 16931 and Peppol grade a large share of their rules as advisory, and &#x60;valid&#x60; ignores those. | [optional] [default to 'fatal']
**ruleset** | **str** | Which ruleset found it — matches an &#x60;id&#x60; in &#x60;rulesets&#x60;. | [optional] [default to 'semantic']

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


