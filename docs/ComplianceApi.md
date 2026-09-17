# invoicepdfs.ComplianceApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**download_document_xml**](ComplianceApi.md#download_document_xml) | **GET** /api/v1/documents/{document_id}/xml | Download Document Xml
[**render_document_xml**](ComplianceApi.md#render_document_xml) | **POST** /api/v1/documents/xml | Render Document Xml
[**validate_compliance**](ComplianceApi.md#validate_compliance) | **POST** /api/v1/documents/validate-compliance | Validate Compliance


# **download_document_xml**
> str download_document_xml(document_id, profile)

Download Document Xml

The e-invoicing XML for a document already stored here.  Reads `data_json` directly rather than going through the render path's reconstruction: the status, the logo and the source document's number are all attached there for the *PDF*, and none of them belong in the XML. The credit note's BG-3 reference is already in the stored payload, resolved when the document was written.

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = invoicepdfs.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = invoicepdfs.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with invoicepdfs.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = invoicepdfs.ComplianceApi(api_client)
    document_id = 'document_id_example' # str | 
    profile = 'peppol_bis_billing_3' # str | Which ruleset to write this against. No default: a document valid under one can be rejected by another, so the choice is the request.

    try:
        # Download Document Xml
        api_response = api_instance.download_document_xml(document_id, profile)
        print("The response of ComplianceApi->download_document_xml:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ComplianceApi->download_document_xml: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | **str**|  | 
 **profile** | **str**| Which ruleset to write this against. No default: a document valid under one can be rejected by another, so the choice is the request. | 

### Return type

**str**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/xml, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | The stored document as XML, in the syntax the chosen profile is expressed in — UBL for Peppol BIS, CII for Factur-X. |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **render_document_xml**
> str render_document_xml(document_compliance_request)

Render Document Xml

The e-invoicing XML for a document, without storing anything.  Takes the same body as `/validate-compliance`, and the pairing is the point: check first, then take the XML once it passes. Nothing here validates against the ruleset — a document missing mandatory fields serialises to XML missing those elements, which is a more useful artefact to look at than a refusal, and `/validate-compliance` is where the refusal belongs.  The syntax is not a parameter. It follows from the profile, because a profile already is a syntax plus a ruleset, and asking a caller for both is asking them to know that Peppol means UBL.

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.document_compliance_request import DocumentComplianceRequest
from invoicepdfs.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = invoicepdfs.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = invoicepdfs.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with invoicepdfs.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = invoicepdfs.ComplianceApi(api_client)
    document_compliance_request = invoicepdfs.DocumentComplianceRequest() # DocumentComplianceRequest | 

    try:
        # Render Document Xml
        api_response = api_instance.render_document_xml(document_compliance_request)
        print("The response of ComplianceApi->render_document_xml:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ComplianceApi->render_document_xml: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_compliance_request** | [**DocumentComplianceRequest**](DocumentComplianceRequest.md)|  | 

### Return type

**str**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/xml, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | The document as XML, in the syntax the chosen profile is expressed in — UBL for Peppol BIS, CII for Factur-X. |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validate_compliance**
> DocumentComplianceResponse validate_compliance(document_compliance_request)

Validate Compliance

Check a document against an e-invoicing ruleset without rendering it.  Costs no renders: nothing is stored and no PDF is produced, so a caller can check every invoice they are about to send rather than discovering the problem from a rejection weeks later.  Two tiers run, and both are reported. The mandatory-field check names a field of the request you can go and change. Schematron then serializes the document and runs the **published rules at a pinned version** over the result — the same artefacts an access point runs — so a finding here quotes the rule id a rejection notice would quote.  Read `valid` together with `fully_checked`: `valid` says nothing fatal was found, and `rulesets` says what actually ran to find it.

### Example

* Bearer Authentication (HTTPBearer):

```python
import invoicepdfs
from invoicepdfs.models.document_compliance_request import DocumentComplianceRequest
from invoicepdfs.models.document_compliance_response import DocumentComplianceResponse
from invoicepdfs.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = invoicepdfs.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = invoicepdfs.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with invoicepdfs.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = invoicepdfs.ComplianceApi(api_client)
    document_compliance_request = invoicepdfs.DocumentComplianceRequest() # DocumentComplianceRequest | 

    try:
        # Validate Compliance
        api_response = api_instance.validate_compliance(document_compliance_request)
        print("The response of ComplianceApi->validate_compliance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ComplianceApi->validate_compliance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_compliance_request** | [**DocumentComplianceRequest**](DocumentComplianceRequest.md)|  | 

### Return type

[**DocumentComplianceResponse**](DocumentComplianceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

