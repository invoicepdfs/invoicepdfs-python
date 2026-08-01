# CursorPagination


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**has_more** | **bool** |  | [optional] [default to False]
**next_cursor** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.cursor_pagination import CursorPagination

# TODO update the JSON string below
json = "{}"
# create an instance of CursorPagination from a JSON string
cursor_pagination_instance = CursorPagination.from_json(json)
# print the JSON string representation of the object
print(CursorPagination.to_json())

# convert the object into a dict
cursor_pagination_dict = cursor_pagination_instance.to_dict()
# create an instance of CursorPagination from a dict
cursor_pagination_from_dict = CursorPagination.from_dict(cursor_pagination_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


