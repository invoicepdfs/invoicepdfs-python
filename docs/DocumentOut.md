# DocumentOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**document_type** | **str** |  | 
**number** | **str** |  | 
**status** | **str** |  | 
**issue_date** | **date** |  | 
**due_date** | **date** |  | [optional] 
**currency** | **str** |  | 
**locale** | **str** |  | [optional] 
**business_profile_id** | **str** |  | 
**customer_id** | **str** |  | 
**source_document_id** | **str** |  | [optional] 
**reason** | **str** |  | [optional] 
**data** | **Dict[str, object]** |  | 
**totals** | [**InvoiceTotalsOut**](InvoiceTotalsOut.md) |  | 
**created_at** | **str** |  | 
**updated_at** | **str** |  | 
**finalized_at** | **str** |  | [optional] 

## Example

```python
from invoicepdfs.models.document_out import DocumentOut

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentOut from a JSON string
document_out_instance = DocumentOut.from_json(json)
# print the JSON string representation of the object
print(DocumentOut.to_json())

# convert the object into a dict
document_out_dict = document_out_instance.to_dict()
# create an instance of DocumentOut from a dict
document_out_from_dict = DocumentOut.from_dict(document_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


