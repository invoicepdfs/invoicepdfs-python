# BatchCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**operation** | **str** |  | [optional] [default to 'render']
**items** | [**List[BatchItemInput]**](BatchItemInput.md) |  | 
**template_id** | **str** |  | [optional] [default to 'tpl_modern']
**output** | [**BatchOutputOptions**](BatchOutputOptions.md) |  | [optional] 

## Example

```python
from invoicepdfs.models.batch_create_request import BatchCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BatchCreateRequest from a JSON string
batch_create_request_instance = BatchCreateRequest.from_json(json)
# print the JSON string representation of the object
print(BatchCreateRequest.to_json())

# convert the object into a dict
batch_create_request_dict = batch_create_request_instance.to_dict()
# create an instance of BatchCreateRequest from a dict
batch_create_request_from_dict = BatchCreateRequest.from_dict(batch_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


