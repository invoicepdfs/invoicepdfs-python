# TemplateDetailResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**TemplateDetail**](TemplateDetail.md) |  | 

## Example

```python
from invoicepdfs.models.template_detail_response import TemplateDetailResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TemplateDetailResponse from a JSON string
template_detail_response_instance = TemplateDetailResponse.from_json(json)
# print the JSON string representation of the object
print(TemplateDetailResponse.to_json())

# convert the object into a dict
template_detail_response_dict = template_detail_response_instance.to_dict()
# create an instance of TemplateDetailResponse from a dict
template_detail_response_from_dict = TemplateDetailResponse.from_dict(template_detail_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


