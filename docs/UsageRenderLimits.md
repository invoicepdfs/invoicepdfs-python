# UsageRenderLimits


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**used** | **int** |  | 
**limit** | **int** |  | 
**remaining** | **int** |  | 

## Example

```python
from invoicepdfs.models.usage_render_limits import UsageRenderLimits

# TODO update the JSON string below
json = "{}"
# create an instance of UsageRenderLimits from a JSON string
usage_render_limits_instance = UsageRenderLimits.from_json(json)
# print the JSON string representation of the object
print(UsageRenderLimits.to_json())

# convert the object into a dict
usage_render_limits_dict = usage_render_limits_instance.to_dict()
# create an instance of UsageRenderLimits from a dict
usage_render_limits_from_dict = UsageRenderLimits.from_dict(usage_render_limits_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


