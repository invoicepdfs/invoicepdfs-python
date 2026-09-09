# ComplianceRulesetOut

One ruleset the document was held to, and whether it actually ran.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**label** | **str** |  | 
**version** | **str** | The upstream release of the rules. Empty for checks with no version of their own. | [optional] [default to '']
**ran** | **bool** | False when this ruleset could not be run at all. A ruleset that did not run is not a pass — &#x60;valid&#x60; only reports what was checked. | 
**reason** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.compliance_ruleset_out import ComplianceRulesetOut

# TODO update the JSON string below
json = "{}"
# create an instance of ComplianceRulesetOut from a JSON string
compliance_ruleset_out_instance = ComplianceRulesetOut.from_json(json)
# print the JSON string representation of the object
print(ComplianceRulesetOut.to_json())

# convert the object into a dict
compliance_ruleset_out_dict = compliance_ruleset_out_instance.to_dict()
# create an instance of ComplianceRulesetOut from a dict
compliance_ruleset_out_from_dict = ComplianceRulesetOut.from_dict(compliance_ruleset_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


