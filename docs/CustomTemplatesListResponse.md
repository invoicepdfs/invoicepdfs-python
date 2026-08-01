# CustomTemplatesListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CustomTemplateOut]**](CustomTemplateOut.md) |  | 
**pagination** | [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.custom_templates_list_response import CustomTemplatesListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CustomTemplatesListResponse from a JSON string
custom_templates_list_response_instance = CustomTemplatesListResponse.from_json(json)
# print the JSON string representation of the object
print(CustomTemplatesListResponse.to_json())

# convert the object into a dict
custom_templates_list_response_dict = custom_templates_list_response_instance.to_dict()
# create an instance of CustomTemplatesListResponse from a dict
custom_templates_list_response_from_dict = CustomTemplatesListResponse.from_dict(custom_templates_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


