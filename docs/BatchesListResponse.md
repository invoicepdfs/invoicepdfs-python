# BatchesListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[BatchOut]**](BatchOut.md) |  | 
**pagination** | [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.batches_list_response import BatchesListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BatchesListResponse from a JSON string
batches_list_response_instance = BatchesListResponse.from_json(json)
# print the JSON string representation of the object
print(BatchesListResponse.to_json())

# convert the object into a dict
batches_list_response_dict = batches_list_response_instance.to_dict()
# create an instance of BatchesListResponse from a dict
batches_list_response_from_dict = BatchesListResponse.from_dict(batches_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


