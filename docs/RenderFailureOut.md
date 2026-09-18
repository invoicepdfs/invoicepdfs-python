# RenderFailureOut

Why a render failed, in the same shape the synchronous path returns.  A synchronous render of a document EN 16931 would reject answers `422 compliance_failed` with every violation at once — a list of fields to go and fill in. A queued render has to be able to say the same thing: the caller who chose `async` did not choose a worse answer.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** | &#x60;compliance_failed&#x60; for a document that is well-formed and would be rejected by the ruleset it asked for; &#x60;unprocessable_entity&#x60; for one the renderer could not make sense of. The same codes the synchronous path returns. | 
**message** | **str** |  | 
**details** | **Dict[str, object]** |  | [optional] 

## Example

```python
from invoicepdfs.models.render_failure_out import RenderFailureOut

# TODO update the JSON string below
json = "{}"
# create an instance of RenderFailureOut from a JSON string
render_failure_out_instance = RenderFailureOut.from_json(json)
# print the JSON string representation of the object
print(RenderFailureOut.to_json())

# convert the object into a dict
render_failure_out_dict = render_failure_out_instance.to_dict()
# create an instance of RenderFailureOut from a dict
render_failure_out_from_dict = RenderFailureOut.from_dict(render_failure_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


