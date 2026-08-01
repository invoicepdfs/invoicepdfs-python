# TemplateDetail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template_id** | **str** |  | 
**name** | **str** |  | 
**document_type** | **str** |  | [optional] [default to 'invoice']
**engine** | **str** |  | 

## Example

```python
from invoicepdfs.models.template_detail import TemplateDetail

# TODO update the JSON string below
json = "{}"
# create an instance of TemplateDetail from a JSON string
template_detail_instance = TemplateDetail.from_json(json)
# print the JSON string representation of the object
print(TemplateDetail.to_json())

# convert the object into a dict
template_detail_dict = template_detail_instance.to_dict()
# create an instance of TemplateDetail from a dict
template_detail_from_dict = TemplateDetail.from_dict(template_detail_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


