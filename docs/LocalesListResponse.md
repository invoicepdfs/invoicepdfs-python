# LocalesListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[LocaleOut]**](LocaleOut.md) |  | 

## Example

```python
from invoicepdfs.models.locales_list_response import LocalesListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of LocalesListResponse from a JSON string
locales_list_response_instance = LocalesListResponse.from_json(json)
# print the JSON string representation of the object
print(LocalesListResponse.to_json())

# convert the object into a dict
locales_list_response_dict = locales_list_response_instance.to_dict()
# create an instance of LocalesListResponse from a dict
locales_list_response_from_dict = LocalesListResponse.from_dict(locales_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


