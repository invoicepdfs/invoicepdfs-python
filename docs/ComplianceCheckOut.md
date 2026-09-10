# ComplianceCheckOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**profile** | **str** |  | 
**ruleset_version** | **str** | The version these rules came from. Worth recording alongside any document you file — rulesets revise, and &#39;which rules did this pass?&#39; is what an audit asks years later. &#x60;rulesets&#x60; breaks the same answer down per ruleset. | 
**valid** | **bool** | Nothing fatal was found. Read it with &#x60;fully_checked&#x60; — on its own it says what was checked came back clean, not that everything was checked. | 
**in_scope** | **bool** | Whether any of these rulesets is likely to apply to this document at all. False when neither party is in a country that uses one — these are European e-invoicing rulesets, and for a wholly domestic US invoice, say, &#x60;valid&#x60; is answering a question nobody asked. Advisory: it never changes the verdict or withholds the check, because an open network means a US seller invoicing a Dutch buyer genuinely needs it. | [optional] [default to True]
**fully_checked** | **bool** | Every ruleset that applies to this profile ran. False means at least one could not, and &#x60;rulesets&#x60; says which and why. | [optional] [default to True]
**rulesets** | [**List[ComplianceRulesetOut]**](ComplianceRulesetOut.md) | Every ruleset the document was held to, including the mandatory-field check, at the version that ran. | [optional] 
**violations** | [**List[ComplianceViolationOut]**](ComplianceViolationOut.md) | Every violation found, not the first — fixing one field per round trip is the experience this avoids. Ordered mandatory-field findings first, since those name a field you can go and change. | [optional] 

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


