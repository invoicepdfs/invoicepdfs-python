# DocumentOutputOptions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**format** | **str** |  | [optional] [default to 'pdf']
**delivery** | **str** |  | [optional] [default to 'url']
**expires_in** | **int** |  | [optional] [default to 3600]

## Example

```python
from invoicepdfs.models.document_output_options import DocumentOutputOptions

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentOutputOptions from a JSON string
document_output_options_instance = DocumentOutputOptions.from_json(json)
# print the JSON string representation of the object
print(DocumentOutputOptions.to_json())

# convert the object into a dict
document_output_options_dict = document_output_options_instance.to_dict()
# create an instance of DocumentOutputOptions from a dict
document_output_options_from_dict = DocumentOutputOptions.from_dict(document_output_options_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


