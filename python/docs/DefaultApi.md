# shinjitsu.DefaultApi

All URIs are relative to *https://api.the-no-corp.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**scan_public_v1_scan_post**](DefaultApi.md#scan_public_v1_scan_post) | **POST** /v1/scan | Scan Public


# **scan_public_v1_scan_post**
> ScanResult scan_public_v1_scan_post(file)

Scan Public

Scan a document for fraud indicators.

Analyzes the uploaded document (PDF or image) and returns a fraud verdict
with supporting indicators. Supports JPEG, PNG images and PDF documents.

**Authentication**: Supports two methods:
- Clerk JWT: `Authorization: Bearer <clerk_jwt>`
- API Token: `Authorization: Bearer shj_...`

**Data retention**: Uploaded files are automatically deleted after 24 hours.

Returns:
- **scan_id**: Unique identifier for this scan
- **verdict**: Overall assessment (clean, suspicious, fraudulent, not_applicable)
- **risk_score**: Risk score from 0.0 (clean) to 1.0 (fraud)
- **indicators**: List of fraud indicators found
- **summary**: Human-readable summary

### Example

* Bearer Authentication (BearerAuth):

```python
import shinjitsu
from shinjitsu.models.scan_result import ScanResult
from shinjitsu.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.the-no-corp.com
# See configuration.py for a list of all supported configuration parameters.
configuration = shinjitsu.Configuration(
    host = "https://api.the-no-corp.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: BearerAuth
configuration = shinjitsu.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with shinjitsu.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = shinjitsu.DefaultApi(api_client)
    file = None # bytearray | Document to analyze (PDF, JPEG, PNG)

    try:
        # Scan Public
        api_response = api_instance.scan_public_v1_scan_post(file)
        print("The response of DefaultApi->scan_public_v1_scan_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->scan_public_v1_scan_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **file** | **bytearray**| Document to analyze (PDF, JPEG, PNG) | 

### Return type

[**ScanResult**](ScanResult.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

