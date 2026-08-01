# ApiRequestLogOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**method** | **str** |  | 
**path** | **str** |  | 
**query** | **str** |  | [optional] 
**status_code** | **int** |  | 
**duration_ms** | **int** |  | [optional] 
**request_body** | **str** |  | [optional] 
**response_body** | **str** |  | [optional] 
**created_at** | **str** |  | 

## Example

```python
from invoicepdfs.models.api_request_log_out import ApiRequestLogOut

# TODO update the JSON string below
json = "{}"
# create an instance of ApiRequestLogOut from a JSON string
api_request_log_out_instance = ApiRequestLogOut.from_json(json)
# print the JSON string representation of the object
print(ApiRequestLogOut.to_json())

# convert the object into a dict
api_request_log_out_dict = api_request_log_out_instance.to_dict()
# create an instance of ApiRequestLogOut from a dict
api_request_log_out_from_dict = ApiRequestLogOut.from_dict(api_request_log_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


