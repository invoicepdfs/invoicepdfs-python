# TemplateVersionCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**label** | **str** |  | [optional] 
**changelog** | **str** |  | [optional] 
**config** | **Dict[str, object]** |  | [optional] 

## Example

```python
from invoicepdfs.models.template_version_create_request import TemplateVersionCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of TemplateVersionCreateRequest from a JSON string
template_version_create_request_instance = TemplateVersionCreateRequest.from_json(json)
# print the JSON string representation of the object
print(TemplateVersionCreateRequest.to_json())

# convert the object into a dict
template_version_create_request_dict = template_version_create_request_instance.to_dict()
# create an instance of TemplateVersionCreateRequest from a dict
template_version_create_request_from_dict = TemplateVersionCreateRequest.from_dict(template_version_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


