# AuthMessageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | **Dict[str, object]** |  | 

## Example

```python
from invoicepdfs.models.auth_message_response import AuthMessageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AuthMessageResponse from a JSON string
auth_message_response_instance = AuthMessageResponse.from_json(json)
# print the JSON string representation of the object
print(AuthMessageResponse.to_json())

# convert the object into a dict
auth_message_response_dict = auth_message_response_instance.to_dict()
# create an instance of AuthMessageResponse from a dict
auth_message_response_from_dict = AuthMessageResponse.from_dict(auth_message_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


