# DocumentCalculateResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**Dict[str, CalculationBreakdown]**](CalculationBreakdown.md) |  | 

## Example

```python
from invoicepdfs.models.document_calculate_response import DocumentCalculateResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentCalculateResponse from a JSON string
document_calculate_response_instance = DocumentCalculateResponse.from_json(json)
# print the JSON string representation of the object
print(DocumentCalculateResponse.to_json())

# convert the object into a dict
document_calculate_response_dict = document_calculate_response_instance.to_dict()
# create an instance of DocumentCalculateResponse from a dict
document_calculate_response_from_dict = DocumentCalculateResponse.from_dict(document_calculate_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


