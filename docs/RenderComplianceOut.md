# RenderComplianceOut

What this PDF was held to, for a render that carries embedded XML.  Absent on a plain `pdf`: no ruleset was applied, so there is no claim to report. A render that was produced at all satisfied every fatal rule that ran — the render is refused otherwise — so the useful questions are which rules those were, and whether all of them ran.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**profile** | **str** | The ruleset this document was built and validated against. | 
**ruleset_version** | **str** | The artefact versions the check actually ran. A profile is held to more than one ruleset, and they are regenerated over time, so this is what makes &#39;which rules did this pass?&#39; answerable later. | 
**fully_checked** | **bool** | False when a ruleset could not run. The document still satisfied everything that did, but the authoritative Schematron tier being absent is a materially weaker statement than it passing. | 
**advisories** | [**List[ComplianceViolationOut]**](ComplianceViolationOut.md) | Non-fatal findings the render proceeded past. Both rulesets grade a large share of their rules as advisory, so these are worth reading and are not a rejection. | [optional] 

## Example

```python
from invoicepdfs.models.render_compliance_out import RenderComplianceOut

# TODO update the JSON string below
json = "{}"
# create an instance of RenderComplianceOut from a JSON string
render_compliance_out_instance = RenderComplianceOut.from_json(json)
# print the JSON string representation of the object
print(RenderComplianceOut.to_json())

# convert the object into a dict
render_compliance_out_dict = render_compliance_out_instance.to_dict()
# create an instance of RenderComplianceOut from a dict
render_compliance_out_from_dict = RenderComplianceOut.from_dict(render_compliance_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


