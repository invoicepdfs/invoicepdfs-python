# BatchItemInput


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**external_id** | **str** |  | [optional] 
**document_type** | **str** |  | [optional] [default to 'invoice']
**data** | **Dict[str, object]** | Document data payload | 

## Example

```python
from invoicepdfs.models.batch_item_input import BatchItemInput

# TODO update the JSON string below
json = "{}"
# create an instance of BatchItemInput from a JSON string
batch_item_input_instance = BatchItemInput.from_json(json)
# print the JSON string representation of the object
print(BatchItemInput.to_json())

# convert the object into a dict
batch_item_input_dict = batch_item_input_instance.to_dict()
# create an instance of BatchItemInput from a dict
batch_item_input_from_dict = BatchItemInput.from_dict(batch_item_input_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


