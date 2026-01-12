# shinjitsu.AnalyzeApi

All URIs are relative to *https://api.the-no-corp.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**analyze_document_v1_analyze_post**](AnalyzeApi.md#analyze_document_v1_analyze_post) | **POST** /v1/analyze | Analyze Document


# **analyze_document_v1_analyze_post**
> AnalyzeResponse analyze_document_v1_analyze_post(authorization, file)

Analyze Document

Analyze a document for fraud indicators.

Requires API token authentication via Authorization header:
```
Authorization: Bearer shj_your_api_token_here
```

Supported file types:
- JPEG images (.jpg, .jpeg)
- PNG images (.png)
- PDF documents (.pdf)

### Example

* Bearer Authentication (BearerAuth):

```python
import shinjitsu
from shinjitsu.models.analyze_response import AnalyzeResponse
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
    api_instance = shinjitsu.AnalyzeApi(api_client)
    authorization = 'authorization_example' # str | Bearer token: 'Bearer shj_...'
    file = None # bytearray | 

    try:
        # Analyze Document
        api_response = api_instance.analyze_document_v1_analyze_post(authorization, file)
        print("The response of AnalyzeApi->analyze_document_v1_analyze_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AnalyzeApi->analyze_document_v1_analyze_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **str**| Bearer token: &#39;Bearer shj_...&#39; | 
 **file** | **bytearray**|  | 

### Return type

[**AnalyzeResponse**](AnalyzeResponse.md)

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

