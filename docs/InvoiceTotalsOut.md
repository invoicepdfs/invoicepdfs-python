# InvoiceTotalsOut


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subtotal** | [**MoneyOut**](MoneyOut.md) |  | 
**discount_total** | [**MoneyOut**](MoneyOut.md) |  | 
**tax_total** | [**MoneyOut**](MoneyOut.md) |  | 
**shipping_total** | [**MoneyOut**](MoneyOut.md) |  | 
**total** | [**MoneyOut**](MoneyOut.md) |  | 

## Example

```python
from invoicepdfs.models.invoice_totals_out import InvoiceTotalsOut

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceTotalsOut from a JSON string
invoice_totals_out_instance = InvoiceTotalsOut.from_json(json)
# print the JSON string representation of the object
print(InvoiceTotalsOut.to_json())

# convert the object into a dict
invoice_totals_out_dict = invoice_totals_out_instance.to_dict()
# create an instance of InvoiceTotalsOut from a dict
invoice_totals_out_from_dict = InvoiceTotalsOut.from_dict(invoice_totals_out_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


