# JobsListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[JobOut]**](JobOut.md) |  | 
**pagination** | [**CursorPagination**](CursorPagination.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.jobs_list_response import JobsListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of JobsListResponse from a JSON string
jobs_list_response_instance = JobsListResponse.from_json(json)
# print the JSON string representation of the object
print(JobsListResponse.to_json())

# convert the object into a dict
jobs_list_response_dict = jobs_list_response_instance.to_dict()
# create an instance of JobsListResponse from a dict
jobs_list_response_from_dict = JobsListResponse.from_dict(jobs_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


