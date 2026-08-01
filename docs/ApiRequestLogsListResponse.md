# ApiRequestLogsListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[ApiRequestLogOut]**](ApiRequestLogOut.md) |  | 

## Example

```python
from invoicepdfs.models.api_request_logs_list_response import ApiRequestLogsListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ApiRequestLogsListResponse from a JSON string
api_request_logs_list_response_instance = ApiRequestLogsListResponse.from_json(json)
# print the JSON string representation of the object
print(ApiRequestLogsListResponse.to_json())

# convert the object into a dict
api_request_logs_list_response_dict = api_request_logs_list_response_instance.to_dict()
# create an instance of ApiRequestLogsListResponse from a dict
api_request_logs_list_response_from_dict = ApiRequestLogsListResponse.from_dict(api_request_logs_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


