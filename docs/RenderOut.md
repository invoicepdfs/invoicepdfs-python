# RenderOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**status** | [**RenderStatus**](RenderStatus.md) |  | 
**document_type** | **str** |  | 
**template_id** | **str** |  | 
**template_version** | **int** |  | [optional] 
**format** | **str** |  | 
**download_url** | **str** |  | [optional] 
**expires_at** | **str** |  | [optional] 
**calculation** | [**CalculationBreakdown**](CalculationBreakdown.md) |  | 
**created_at** | **str** |  | 
**compliance** | [**RenderComplianceOut**](RenderComplianceOut.md) |  | [optional] 
**failure** | [**RenderFailureOut**](RenderFailureOut.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.render_out import RenderOut

# TODO update the JSON string below
json = "{}"
# create an instance of RenderOut from a JSON string
render_out_instance = RenderOut.from_json(json)
# print the JSON string representation of the object
print(RenderOut.to_json())

# convert the object into a dict
render_out_dict = render_out_instance.to_dict()
# create an instance of RenderOut from a dict
render_out_from_dict = RenderOut.from_dict(render_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


