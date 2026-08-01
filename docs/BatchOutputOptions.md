# BatchOutputOptions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**format** | **str** |  | [optional] [default to 'pdf']
**combine** | **bool** |  | [optional] [default to False]
**archive_format** | **str** |  | [optional] [default to 'zip']

## Example

```python
from invoicepdfs.models.batch_output_options import BatchOutputOptions

# TODO update the JSON string below
json = "{}"
# create an instance of BatchOutputOptions from a JSON string
batch_output_options_instance = BatchOutputOptions.from_json(json)
# print the JSON string representation of the object
print(BatchOutputOptions.to_json())

# convert the object into a dict
batch_output_options_dict = batch_output_options_instance.to_dict()
# create an instance of BatchOutputOptions from a dict
batch_output_options_from_dict = BatchOutputOptions.from_dict(batch_output_options_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


