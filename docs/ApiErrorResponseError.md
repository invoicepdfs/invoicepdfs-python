# ApiErrorResponseError


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | 
**message** | **str** |  | 
**request_id** | **str** | Trace id for this request; also returned as X-Trace-Id. | [optional] 
**details** | **object** | Error-specific context. Validation failures carry &#x60;fields&#x60;. | [optional] 

## Example

```python
from invoicepdfs.models.api_error_response_error import ApiErrorResponseError

# TODO update the JSON string below
json = "{}"
# create an instance of ApiErrorResponseError from a JSON string
api_error_response_error_instance = ApiErrorResponseError.from_json(json)
# print the JSON string representation of the object
print(ApiErrorResponseError.to_json())

# convert the object into a dict
api_error_response_error_dict = api_error_response_error_instance.to_dict()
# create an instance of ApiErrorResponseError from a dict
api_error_response_error_from_dict = ApiErrorResponseError.from_dict(api_error_response_error_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


