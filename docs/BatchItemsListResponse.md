# BatchItemsListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BatchItemOut]**](BatchItemOut.md) |  | 
**pagination** | [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.batch_items_list_response import BatchItemsListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BatchItemsListResponse from a JSON string
batch_items_list_response_instance = BatchItemsListResponse.from_json(json)
# print the JSON string representation of the object
print(BatchItemsListResponse.to_json())

# convert the object into a dict
batch_items_list_response_dict = batch_items_list_response_instance.to_dict()
# create an instance of BatchItemsListResponse from a dict
batch_items_list_response_from_dict = BatchItemsListResponse.from_dict(batch_items_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


