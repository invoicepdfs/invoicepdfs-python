# PageSizesListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[PageSizeOut]**](PageSizeOut.md) |  | 

## Example

```python
from invoicepdfs.models.page_sizes_list_response import PageSizesListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PageSizesListResponse from a JSON string
page_sizes_list_response_instance = PageSizesListResponse.from_json(json)
# print the JSON string representation of the object
print(PageSizesListResponse.to_json())

# convert the object into a dict
page_sizes_list_response_dict = page_sizes_list_response_instance.to_dict()
# create an instance of PageSizesListResponse from a dict
page_sizes_list_response_from_dict = PageSizesListResponse.from_dict(page_sizes_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


