# TemplateCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**description** | **str** |  | [optional] 
**base_template_id** | **str** |  | [optional] [default to 'tpl_modern']
**config** | **Dict[str, object]** |  | [optional] 

## Example

```python
from invoicepdfs.models.template_create_request import TemplateCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TemplateCreateRequest from a JSON string
template_create_request_instance = TemplateCreateRequest.from_json(json)
# print the JSON string representation of the object
print(TemplateCreateRequest.to_json())

# convert the object into a dict
template_create_request_dict = template_create_request_instance.to_dict()
# create an instance of TemplateCreateRequest from a dict
template_create_request_from_dict = TemplateCreateRequest.from_dict(template_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


