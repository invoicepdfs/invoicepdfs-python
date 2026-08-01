# CustomTemplateOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**name** | **str** |  | 
**description** | **str** |  | [optional] 
**base_template_id** | **str** |  | 
**config** | **Dict[str, object]** |  | [optional] 
**status** | **str** |  | 
**is_default** | **bool** |  | [optional] [default to False]
**created_at** | **str** |  | 
**updated_at** | **str** |  | 
**published_at** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.custom_template_out import CustomTemplateOut

# TODO update the JSON string below
json = "{}"
# create an instance of CustomTemplateOut from a JSON string
custom_template_out_instance = CustomTemplateOut.from_json(json)
# print the JSON string representation of the object
print(CustomTemplateOut.to_json())

# convert the object into a dict
custom_template_out_dict = custom_template_out_instance.to_dict()
# create an instance of CustomTemplateOut from a dict
custom_template_out_from_dict = CustomTemplateOut.from_dict(custom_template_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


