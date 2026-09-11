# CodeListResponse

A coded list from a standard, and whether it is the whole of one.  `exhaustive` is the field that changes what a client does. `true` means a value outside `data` is wrong, so the list can back a picker with no escape hatch. `false` means `data` is a shortlist of the codes an invoice usually needs — the API accepts any code, nothing validates against this, and treating it as closed rejects values that are perfectly valid.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CodeOut]**](CodeOut.md) |  | 
**standard** | **str** | The code list these values come from. | 
**exhaustive** | **bool** | Whether &#x60;data&#x60; is the complete list. When false it is a shortlist and other codes remain valid. | 

## Example

```python
from invoicepdfs.models.code_list_response import CodeListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CodeListResponse from a JSON string
code_list_response_instance = CodeListResponse.from_json(json)
# print the JSON string representation of the object
print(CodeListResponse.to_json())

# convert the object into a dict
code_list_response_dict = code_list_response_instance.to_dict()
# create an instance of CodeListResponse from a dict
code_list_response_from_dict = CodeListResponse.from_dict(code_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


