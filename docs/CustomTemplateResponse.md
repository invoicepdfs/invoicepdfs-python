# CustomTemplateResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CustomTemplateOut**](CustomTemplateOut.md) |  | 

## Example

```python
from invoicepdfs.models.custom_template_response import CustomTemplateResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CustomTemplateResponse from a JSON string
custom_template_response_instance = CustomTemplateResponse.from_json(json)
# print the JSON string representation of the object
print(CustomTemplateResponse.to_json())

# convert the object into a dict
custom_template_response_dict = custom_template_response_instance.to_dict()
# create an instance of CustomTemplateResponse from a dict
custom_template_response_from_dict = CustomTemplateResponse.from_dict(custom_template_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


