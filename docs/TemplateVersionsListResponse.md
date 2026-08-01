# TemplateVersionsListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[TemplateVersionOut]**](TemplateVersionOut.md) |  | 

## Example

```python
from invoicepdfs.models.template_versions_list_response import TemplateVersionsListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TemplateVersionsListResponse from a JSON string
template_versions_list_response_instance = TemplateVersionsListResponse.from_json(json)
# print the JSON string representation of the object
print(TemplateVersionsListResponse.to_json())

# convert the object into a dict
template_versions_list_response_dict = template_versions_list_response_instance.to_dict()
# create an instance of TemplateVersionsListResponse from a dict
template_versions_list_response_from_dict = TemplateVersionsListResponse.from_dict(template_versions_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


