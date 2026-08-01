# TemplateVersionOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**template_id** | **str** |  | 
**version** | **int** |  | 
**label** | **str** |  | [optional] 
**changelog** | **str** |  | [optional] 
**config** | **Dict[str, object]** |  | 
**created_at** | **str** |  | 

## Example

```python
from invoicepdfs.models.template_version_out import TemplateVersionOut

# TODO update the JSON string below
json = "{}"
# create an instance of TemplateVersionOut from a JSON string
template_version_out_instance = TemplateVersionOut.from_json(json)
# print the JSON string representation of the object
print(TemplateVersionOut.to_json())

# convert the object into a dict
template_version_out_dict = template_version_out_instance.to_dict()
# create an instance of TemplateVersionOut from a dict
template_version_out_from_dict = TemplateVersionOut.from_dict(template_version_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


